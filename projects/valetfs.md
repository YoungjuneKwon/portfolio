# ValetFS — zero-knowledge secrets vault

**Go · FUSE · end-to-end encryption · Cloudflare Durable Objects · React Native**

Your credentials live on your phone. A daemon on the workstation serves them **in memory only**,
and only while the phone allows it. Nothing is written to the machine's disk.

- Daemon and CLI: open source — https://github.com/winm2m/valet-fs
- iOS client: shipped on the App Store, 7 languages

## Why it exists

Developer machines accumulate credentials — `.env` files, `~/.aws/credentials`, service-account
JSON, signing keys — and they persist long after they should. Laptop theft, a stray backup, or a
compromised build script turns a directory listing into a breach. Vault products solve this for
companies with an identity platform; they do not solve it for one person with four machines.

ValetFS inverts custody: the phone is the vault, the workstation is a temporary consumer.

## Engineering

**Transport and custody.** Secrets are end-to-end encrypted between phone and daemon. The relay
never sees plaintext. The daemon holds decrypted material in process memory and wipes it on lock,
disconnect, or grace expiry.

**Control plane.** A WebSocket control plane on Cloudflare Durable Objects gives each session a
single consistent coordination point — pairing, presence, push, and revocation — without running
stateful servers.

**Filesystem.** A FUSE mount when `/dev/fuse` is available, with automatic fallback to a loopback
WebDAV server when it is not (containers, restricted hosts). The same CLI works either way, so
consumers do not have to care which backend is active.

**Grace and revocation.** The daemon runs on a configurable grace timer. When the phone
disconnects, secrets survive for the grace window and are then wiped — so a closed laptop lid does
not mean re-pairing, but a lost machine does not stay armed indefinitely.

**Mobile client.** React Native / Expo with native modules, built and released through EAS,
localized into 7 languages, and taken through App Store review.

**Security work.** A full security audit produced 15 findings across the protocol and client;
all were fixed and shipped, including a protocol version bump with a migration path for
already-paired devices.

## Business model

Open core: the daemon and CLI are free and open source; the iOS convenience client is sold through
Apple In-App Purchase.
