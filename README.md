# Youngjune Kwon — Engineering Portfolio

Full-cycle product engineer based in Seoul (KST, UTC+9). 20+ years in software.

I ship end to end on my own: product design → implementation → infrastructure → billing →
App Store review → operations.

`#Go` `#Rust` `#Python` `#TypeScript` `#JavaScript` `#Solidity` `#Swift` `#Java` `#Shell`
`#iOS` `#Android` `#macOS` `#Windows` `#Linux` `#Docker` `#Chrome` `#Web`

- Email — yjkwon@winm2m.com
- LinkedIn — https://www.linkedin.com/in/youngjune-kwon-b21571265/
- GitHub — https://github.com/YoungjuneKwon · https://github.com/winm2m

Descriptions below are quoted from each project's own README or store listing.

---

## 1. Shipped products

### iOS apps (App Store)

**[ValetFS](https://apps.apple.com/kr/app/valetfs/id6804526734)** — v1.1.2 · released 2026-08-31 · Developer Tools · 7 languages
`#Go` `#TypeScript` `#ReactNative` `#iOS` `#macOS` `#Linux`

> "Keep API keys on your phone and lend them to an AI agent's machine — in memory only, never on
> disk, and only while you allow it."

Daemon and CLI are open source: [winm2m/valet-fs](https://github.com/winm2m/valet-fs).

**[Sidera — 사주와 별자리](https://apps.apple.com/kr/app/id6806914044)** — v1.4.0 · released 2026-09-03 · Lifestyle
`#Python` `#FastAPI` `#TypeScript` `#Expo` `#iOS`

> "출생 차트를 결정론적으로 계산하고, 그 결과를 근거로 LLM이 해석해 주는 점성술 앱."
> (An astrology app that computes the natal chart deterministically and has an LLM interpret the
> computed result.)

Source is private. Backend: FastAPI + SQLAlchemy. Mobile: Expo SDK 54 + expo-router.
The astronomy engine is dependency-free pure Python, because an LLM cannot compute celestial
positions and will hallucinate them.

### Web product

**[Proveri](https://proveri.ai)** — survey and statistics SaaS
`#Python` `#FastAPI` `#PostgreSQL` `#TypeScript` `#React` `#Web`

> "Surveys with publication-ready statistics."

Paddle merchant-of-record and Apple IAP billing; GCP Cloud Run and Cloudflare infrastructure.
Source is private.

### npm packages

| Package | Version | Description (from README) |
|---|---|---|
| [@winm2m/inferential-stats-js](https://www.npmjs.com/package/@winm2m/inferential-stats-js) | 1.9.0 | "A headless JavaScript SDK for advanced statistical analysis in the browser using WebAssembly (Pyodide). Performs SPSS-level inferential statistics entirely client-side with no backend required." |
| [@winm2m/react-stats-ui](https://www.npmjs.com/package/@winm2m/react-stats-ui) | 0.22.2 | "React UI component for browser-based inferential statistics workflows, powered by `@winm2m/inferential-stats-js`." |
| [@winm2m/react-data-workspace](https://www.npmjs.com/package/@winm2m/react-data-workspace) | 0.10.0 | "Composable data workspace shell that embeds `@winm2m/react-stats-ui` plugins" |
| [@texo-ui/react](https://www.npmjs.com/package/@texo-ui/react) | 0.2.0 | "React renderer for Texo: reconciles a streaming UI tree into your components." |
| [@texo-ui/standalone](https://www.npmjs.com/package/@texo-ui/standalone) | 0.2.0 | "Texo in one script tag. Self-contained bundle for CDN and no-build pages." |
| [@texo-ui/data-adapter](https://www.npmjs.com/package/@texo-ui/data-adapter) | 0.2.0 | "Bring-your-own-storage drivers for Texo: local, Google Drive, Notion, HTTP." |

`#TypeScript` `#React` `#WebAssembly` `#Web`

### PyPI package

**[leanprompt](https://pypi.org/project/leanprompt/)** — 0.4.4 · 13 releases · MIT
`#Python` `#FastAPI`

> "A lightweight, engineering-first LLM framework for FastAPI featuring session-based context
> caching and reliable output validation."

### Docker Hub images

| Image | Pulls | Description (from README / listing) |
|---|---|---|
| [winm2m/fluxmask-nginx](https://hub.docker.com/r/winm2m/fluxmask-nginx) | 736 | "This Docker image provides Nginx with the Flux-Mask Lua plugin pre-installed and configured." |
| [winm2m/opencode](https://hub.docker.com/r/winm2m/opencode) | 577 | "A ready-to-use Docker image for running OpenCode with all necessary models and dependencies pre-downloaded." |
| [winm2m/email-forward](https://hub.docker.com/r/winm2m/email-forward) | 119 | "A Docker image that forwards emails received to the specified host to another address." |

`#Docker` `#Linux` `#Nginx` `#Lua`

---

## 2. Public repositories — timeline

Reverse chronological. Forks of third-party projects are omitted.

### 2026

**[winm2m/valet-fs](https://github.com/winm2m/valet-fs)** · 2026-09 · `#Go` `#FUSE` `#WebDAV` `#macOS` `#Linux`
> "Keep API keys on your phone and lend them to an AI agent's machine — in memory only, never on disk, and only while you allow it."

**[winm2m/texo-ui](https://github.com/winm2m/texo-ui)** · 2026-09 · `#TypeScript` `#React` `#Web`
> "Weave Text into UI. A stream-oriented Generatable UI framework for the LLM era."
>
> "Unlike Vercel's `v0` or standard generative UI tools that rely on brittle JSON or raw HTML
> generation, Texo uses a robust, human-readable syntax (Markdown Directives + YAML) to 'weave'
> UI components in real-time."

**[winm2m/inferential-stats-js](https://github.com/winm2m/inferential-stats-js)** · 2026-09 · `#TypeScript` `#WebAssembly` `#Web`
**[winm2m/react-stats-ui](https://github.com/winm2m/react-stats-ui)** · 2026-09 · `#TypeScript` `#React` `#Web`
> See npm table above.

**[diligent-hours](https://github.com/YoungjuneKwon/diligent-hours)** · 2026-08 · `#Rust` `#Tauri` `#Windows` `#macOS`
> "A desktop timer that treats your first keyboard/mouse input of the day as the start of work,
> then shows the time remaining until the agreed workday is over and alerts you when it ends."

**[claude-voice](https://github.com/YoungjuneKwon/claude-voice)** · 2026-08 · `#Python` `#Linux`
> "Hear what Claude Code just did, and answer it out loud — without opening the laptop. Every time
> a Claude Code turn ends, its response is summarized into a few sentences written for the ear and
> pushed to Telegram. Reply there by voice and the session picks up where it left off."

**[market-orchestrator](https://github.com/YoungjuneKwon/market-orchestrator)** · 2026-07 · `#Python` `#NodeJS` `#Vite` `#Linux`
> "Python + Node.js based monorepo for automated trading operations with a broker-agnostic
> architecture. … Start with Korea Investment & Securities (KIS) Open API, but keep broker
> integrations pluggable. Provide safety-first controls such as forced stop-loss sell and
> emergency stop."

**[dockerimage-winm2m-opencode](https://github.com/YoungjuneKwon/dockerimage-winm2m-opencode)** · 2026-07 · ★1 · `#Docker` `#Linux`
> "A ready-to-use Docker image for running OpenCode with all necessary models and dependencies
> pre-downloaded. … Automatically built and pushed to Docker Hub on every Dockerfile update."

**[forked-semopy](https://github.com/YoungjuneKwon/forked-semopy)** · 2026-07 · ★13 · `#Python`
> "semopy is an umbrella Python package that includes numerous Structural Equation Modelling (SEM)
> techniques."

A maintained fork of [semopy](https://bitbucket.org/herrberg/semopy). Most-starred repository.

**[winm2m/react-data-workspace](https://github.com/winm2m/react-data-workspace)** · 2026-05 · `#TypeScript` `#React` `#Web`

**[winm2m/leanprompt](https://github.com/winm2m/leanprompt)** · 2026-05 · `#Python` `#FastAPI`
> "A lightweight, engineering-first LLM framework for FastAPI featuring session-based context
> caching and reliable output validation."

**[shadow-translate-bridge](https://github.com/YoungjuneKwon/shadow-translate-bridge)** · 2026-03 · `#TypeScript` `#Web`
> "A lightweight bridge to sync Shadow DOM content with browser translation engines (like Google
> Translate)."

**[winm2m/leanprompt-client](https://github.com/winm2m/leanprompt-client)** · 2026-02 · `#TypeScript` `#React` `#Web`
> "A React client library for LeanPrompt, providing seamless WebSocket synchronization and
> streaming hooks for AI-driven applications."

**[just-replace-http](https://github.com/YoungjuneKwon/just-replace-http)** · 2026-02 · `#JavaScript` `#Chrome`
> "A Chrome extension that replaces parts of HTTP request strings with desired strings before
> sending the request. … Regex pattern matching and group references. … Provides Requestly-style
> replace functionality for free. … UI language automatically adapts to your Chrome browser
> language (English, French, Spanish, Arabic, Chinese, Russian, Korean)."

### 2025

**[flux-mask-clients](https://github.com/YoungjuneKwon/flux-mask-clients)** · 2025-12 · `#TypeScript` `#Web`
> "Client-side libraries for Flux-Mask encryption. … `@flux-mask/core`: Core encryption utilities
> and shared types. `@flux-mask/axios-interceptor`: Axios interceptor for automatic
> request/response encryption. `@flux-mask/fetch-wrapper`: Fetch API wrapper with built-in
> encryption."

Server side ships as the `winm2m/fluxmask-nginx` Docker image above.

**[froala-under-closed-shadowroot](https://github.com/YoungjuneKwon/froala-under-closed-shadowroot)** · 2025-11 · `#JavaScript` `#Web`
> "Sample code for using Froala WYSIWYG editor under a closed shadow root."

**[signal-factory](https://github.com/YoungjuneKwon/signal-factory)** · 2025-11
> "Signal Factory - 상세 기획 문서."

**[product-2025-report-email-consultation](https://github.com/YoungjuneKwon/product-2025-report-email-consultation)** · 2025-10 · `#Python`
> "Gmail 상담 메일을 수집하고 Excel 보고서를 생성하는 Python 프로젝트."

**[tailwind-shadcn-webcomponent](https://github.com/YoungjuneKwon/tailwind-shadcn-webcomponent)** · 2025-08 · `#Web`

**[product-2025-pretty-textarea](https://github.com/YoungjuneKwon/product-2025-pretty-textarea)** · 2025-06 · `#JavaScript` `#Web`
> "Textarea component which can be formatted by rule."

**[cloudflare-worker-mqtt-relay](https://github.com/YoungjuneKwon/cloudflare-worker-mqtt-relay)** · 2025-04 · ★3 · `#JavaScript` `#Cloudflare`
> "A relay server that allows you to perform simple communication with external MQTT servers in
> Cloudflare Worker."

**[ios-native-boost-webview](https://github.com/YoungjuneKwon/ios-native-boost-webview)** · 2025-01 · `#Swift` `#iOS`

### 2024 and earlier

**[android-nativeboost-webview](https://github.com/YoungjuneKwon/android-nativeboost-webview)** · 2024-12 · `#Java` `#Android`
> "Webview inherated View class for enhancing performance of loading web resource."

**[product-2024-general-web](https://github.com/YoungjuneKwon/product-2024-general-web)** · 2024-09 · `#JavaScript` `#Web`
> "This package is a set of features commonly used to build web-based applications. It includes
> utility functions related to JWT authentication…"

**[winm2m-docker-tunnel](https://github.com/YoungjuneKwon/winm2m-docker-tunnel)** · 2023-05 · `#Docker` `#Linux`
> "A docker image for opening ssh tunnel."

**[colab_tools](https://github.com/YoungjuneKwon/colab_tools)** · 2023-04 · `#Python`

**[winm2m-cfworker-base](https://github.com/YoungjuneKwon/winm2m-cfworker-base)** · 2023-01 · `#JavaScript` `#Cloudflare`
> "A library for creating basic CRUD endpoints for Cloudflare Workers. It use a notion page as
> database."

**[product-2022-argos-api-js](https://github.com/YoungjuneKwon/product-2022-argos-api-js)** · 2022-11 · `#JavaScript`

**[docker-sendmail-forward](https://github.com/YoungjuneKwon/docker-sendmail-forward)** · 2022-11 · `#Shell` `#Docker` `#Linux`
> "A Docker image that forwards emails received to the specified host to another address."

**[solidity-samples](https://github.com/YoungjuneKwon/solidity-samples)** · 2022-09 · `#Solidity` `#Ethereum`

Cross-contract call samples. See [NFT Minting Platform](projects/nft-minting.md) for the
production Solidity work from the same period.

**[iotcam-android](https://github.com/YoungjuneKwon/iotcam-android)** · 2022-05 · `#Java` `#Android`
> "IoT CAM Android."

**[generate-self-signed-cert](https://github.com/YoungjuneKwon/generate-self-signed-cert)** · 2021-07 · `#Shell` `#Linux`
> "./0_generate_root_ca.sh org_name"

**[daily-coding](https://github.com/YoungjuneKwon/daily-coding)** · 2021-04 · `#Python` `#Jupyter`

**[automation_si4n](https://github.com/YoungjuneKwon/automation_si4n)** · 2021-03 · `#Python`

**[dockers](https://github.com/YoungjuneKwon/dockers)** · 2021-02 · `#Docker` `#Linux`

**[python-batch-resize](https://github.com/YoungjuneKwon/python-batch-resize)** · 2020-09 · `#Python`
> "Resize and crop all images stored in the folder. By designating a specific folder, resize and
> crop all images in the sub folders of the specified folder."

**[practice-math-vue](https://github.com/YoungjuneKwon/practice-math-vue)** · 2020-01 · `#JavaScript` `#Vue` `#Web`

**[argos-rpi-python](https://github.com/YoungjuneKwon/argos-rpi-python)** · 2019-05 · `#Python` `#RaspberryPi`
> "Python package for processing GPIO on RaspberryPI."

**[esp32-toolchain-rpi](https://github.com/YoungjuneKwon/esp32-toolchain-rpi)** · 2019-05 · ★2 · `#Shell` `#ESP32` `#RaspberryPi`
> "This is the build script and binary of the toolchain for RPi in the ESP-IDF installation guide."

**[konlpy-rest](https://github.com/YoungjuneKwon/konlpy-rest)** · 2019-04 · `#Python`
> "KoNLPy를 웹 어플리케이션에서 활용할 수 있도록 만든 간단한 REST API 서비스입니다."

**[RemoteWebMouse](https://github.com/YoungjuneKwon/RemoteWebMouse)** · 2019-01

**[argos-streamer](https://github.com/YoungjuneKwon/argos-streamer)** · 2018-12 · `#JavaScript` `#MQTT`
> "Server application for streaming MQTT packets. Take specific topics and keep them in files for
> a certain period of time under a specific folder."

---

## 3. Deep dive

- **[NFT Minting Platform](projects/nft-minting.md)** — ERC-721 launch system with Merkle-proof
  allowlist and on-chain anti-bot controls (2022, client engagement). Source is private; the
  document describes the engineering approach only.
  `#Solidity` `#Ethereum` `#Vue` `#Web3`
