# NFT Minting Platform — ERC-721 launch system

**2022 · Client engagement for a Korean NFT startup · Solidity, Vue 3, Web3**

> Source code is not public. This document describes the engineering approach only; no client
> assets, addresses, or proprietary material are included.

I designed and built the full launch stack for an Ethereum NFT collection: the ERC-721 contract,
the public minting site, and the back office used to operate the sale.

## The problem a mint has to solve

A public NFT mint is a short, adversarial event. Thousands of wallets compete for a fixed supply
in a few minutes, and a meaningful share of them are bots. Everything that matters happens in a
window too small to fix by hand, and every rule has to be enforced on-chain because the frontend
cannot be trusted. That makes it, in practice, an access-control and rate-limiting problem with
money attached.

## Contract design

Built on OpenZeppelin `ERC721`, `Ownable`, `Strings`, and `MerkleProof`.

**Merkle-proof allowlist.** Storing thousands of allowlisted addresses on-chain is prohibitively
expensive. Instead, the contract stores a single 32-byte Merkle root; each caller supplies a proof
that `keccak256(msg.sender)` is a leaf under that root. Proofs are generated off-chain with
`merkletreejs` and `keccak256` using sorted pairs, then distributed to eligible wallets. Cost of
verification is logarithmic in the allowlist size, and the allowlist can be rotated by replacing
the root in one transaction.

**Anti-bot interval.** Each address's last minting block is recorded, and a subsequent call is
rejected unless `lastCallBlockNumber[msg.sender] + antibotInterval < block.number`. This forces a
cooldown measured in blocks rather than wall-clock time, so it cannot be gamed by timestamp
manipulation. The interval is operator-tunable during the sale.

**Layered supply limits.** Four independent constraints are enforced on every mint, per price plan:
total supply for the plan, maximum tokens per transaction, maximum tokens per wallet, and a sale
start block. Each is a separate `require` with a distinct revert reason, so failures are
diagnosable from the transaction receipt alone rather than by guesswork.

**Multi-tier pricing.** Price plans are stored as an array with an index indirection — a
whitelist plan and a public plan are selected by index, so the operator can switch pricing tiers
mid-sale without redeploying. Each minted token records the plan it was sold under, which makes
post-sale accounting (refunds, per-tier revenue) possible on-chain.

**Exact-payment check.** `msg.value` must equal `unitPrice × requestedCount` exactly. Accepting
overpayment would create a refund obligation with no clean on-chain path to settle it.

**Reveal mechanism.** Before reveal, `tokenURI` returns a single placeholder URI for every token;
after the operator flips the flag, it returns per-token metadata. This prevents rarity sniping
during the mint, when metadata would otherwise let bots pick valuable tokens.

**Two-tier authorization.** `owner` and a mutable `managers` array are separated: operational
functions (pricing, reveal, Merkle root, sale parameters) are available to managers, while
`withdraw` is restricted to the owner alone. Day-to-day operators never hold the key that can move
funds.

**Operational recovery.** Batch airdrop, reclaim-from-address, and burn-range functions were
included for failed or disputed mints — with the unique-minter counter kept consistent across
every path that changes a balance.

## Frontend

Vue 3 + Quasar single-page application. Wallet connection, live sale state read from the contract
(`getInformation` returns the full sale state in one call to minimize RPC round-trips), Merkle
proof lookup for the connected address, and transaction submission with error surfacing mapped
from the contract's revert reasons. Node polyfills (`crypto-browserify`, `stream-browserify`,
`buffer`) were required to run the web3 cryptography stack in the browser.

A separate back-office application handled allowlist management, sale configuration, and
monitoring during the event.

## What transfers

The NFT market this was built for has since collapsed, but the engineering did not. On-chain
access control, Merkle-based eligibility proofs, block-level rate limiting, operator/owner
privilege separation, and exact-value payment validation are the same primitives that regulated
token issuance, tokenized real-world assets, and on-chain settlement systems are built from —
and they are the same surfaces that smart contract audits examine first.
