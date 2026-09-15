<div align="center">

# Youngjune Kwon

**Full-cycle product engineer** · Seoul, Korea (KST, UTC+9) · 20+ years in software

[![Email](https://img.shields.io/badge/email-yjkwon%40winm2m.com-0A66C2?style=flat-square&logo=maildotru&logoColor=white)](mailto:yjkwon@winm2m.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-youngjune--kwon-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/youngjune-kwon-b21571265/)
[![GitHub](https://img.shields.io/badge/GitHub-YoungjuneKwon-181717?style=flat-square&logo=github)](https://github.com/YoungjuneKwon)

![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Solidity](https://img.shields.io/badge/Solidity-363636?style=flat-square&logo=solidity&logoColor=white)
![Swift](https://img.shields.io/badge/Swift-F05138?style=flat-square&logo=swift&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white)
![iOS](https://img.shields.io/badge/iOS-000000?style=flat-square&logo=apple&logoColor=white)

**2 apps on the App Store · 19 packages on npm · 1 on PyPI · 3 images on Docker Hub**

</div>

I ship end to end on my own: product design → implementation → infrastructure → billing →
App Store review → operations.

> Descriptions below are quoted from each project's own README, package manifest, or store listing.

---

## 1. Shipped products

### iOS apps

<table>
<tr>
<td width="110" align="center">
<a href="https://apps.apple.com/kr/app/valetfs/id6804526734">
<img src="https://is1-ssl.mzstatic.com/image/thumb/Purple221/v4/ff/e1/16/ffe1167d-db41-b821-d5c0-55a92f8c3a8c/AppIcon-0-0-1x_U007ephone-0-1-85-220.png/512x512bb.jpg" width="96"><br>
<b>ValetFS</b></a>
</td>
<td>

**[ValetFS](https://apps.apple.com/kr/app/valetfs/id6804526734)** · v1.1.2 · released 2026-08-31 · Developer Tools · 7 languages

> "Keep API keys on your phone and lend them to an AI agent's machine — in memory only, never on
> disk, and only while you allow it."
>
> "ValetFS is a Zero-Backend, P2P, in-memory virtual file system that exposes short-lived tokens
> and keys to AI agents only while a paired mobile app allows it."

`Go` `FUSE` `WebDAV` `WebRTC (pion)` `Cloudflare Worker` `React Native` · `iOS` `macOS` `Linux`
Daemon and CLI open source → [winm2m/valet-fs](https://github.com/winm2m/valet-fs)

</td>
</tr>
</table>

<div align="center">
<img src="https://raw.githubusercontent.com/WinM2M/valet-fs/main/docs/media/memory-not-disk.png" width="440">
<img src="https://raw.githubusercontent.com/WinM2M/valet-fs/main/docs/media/valet-stand.png" width="440">
<br>
<img src="https://is1-ssl.mzstatic.com/image/thumb/PurpleSource221/v4/2e/fc/d8/2efcd88e-938f-4f21-c68d-fe81754d9d93/01-home.png/320x480bb.jpg" width="185">
<img src="https://is1-ssl.mzstatic.com/image/thumb/PurpleSource221/v4/a9/88/1b/a9881b94-77be-d3cb-1e9b-ca53c83eac10/02-session.png/320x480bb.jpg" width="185">
<img src="https://is1-ssl.mzstatic.com/image/thumb/PurpleSource211/v4/52/32/ae/5232aeb3-a943-00e9-9943-8f3bf74f1915/03-new-secret.png/320x480bb.jpg" width="185">
<img src="https://is1-ssl.mzstatic.com/image/thumb/PurpleSource221/v4/ba/c1/23/bac12366-45b7-2f3a-7da4-6ab77cb95fcf/04-pair.png/320x480bb.jpg" width="185">
</div>

<table>
<tr>
<td width="110" align="center">
<a href="https://apps.apple.com/kr/app/id6806914044">
<img src="https://is1-ssl.mzstatic.com/image/thumb/Purple221/v4/b6/21/13/b62113b2-7c41-ee2e-4b5e-c034444d767f/AppIcon-0-0-1x_U007ephone-0-1-85-220.png/512x512bb.jpg" width="96"><br>
<b>Sidera</b></a>
</td>
<td>

**[Sidera — 사주와 별자리](https://apps.apple.com/kr/app/id6806914044)** · v1.4.0 · released 2026-09-03 · Lifestyle
**Contract development** — built end to end for a client and published under their App Store account.

> "출생 차트를 결정론적으로 계산하고, 그 결과를 근거로 LLM이 해석해 주는 점성술 앱."
> *(An astrology app that computes the natal chart deterministically and has an LLM interpret the
> computed result.)*

`Python` `FastAPI` `SQLAlchemy` `TypeScript` `Expo SDK 54` · `iOS`
Source is the client's and stays private. The astronomy engine is dependency-free pure Python —
an LLM cannot compute celestial positions and will hallucinate them, so the backend owns the
calculation and the model only interprets its output.

</td>
</tr>
</table>

<div align="center">
<img src="https://is1-ssl.mzstatic.com/image/thumb/PurpleSource211/v4/df/80/c7/df80c78e-02e6-f45c-2942-2125f93f68ff/6.9-1-chat.png/320x480bb.jpg" width="185">
<img src="https://is1-ssl.mzstatic.com/image/thumb/PurpleSource221/v4/8b/98/b6/8b98b6bf-822b-a527-fc51-4c15560087f7/6.9-2-answer.png/320x480bb.jpg" width="185">
<img src="https://is1-ssl.mzstatic.com/image/thumb/PurpleSource221/v4/31/a0/8e/31a08e5c-45ae-3a02-7ac5-654c17af2933/6.9-3-chart.png/320x480bb.jpg" width="185">
<img src="https://is1-ssl.mzstatic.com/image/thumb/PurpleSource221/v4/a9/12/6c/a9126c35-3156-77a6-cb04-4715abf070f8/6.9-4-credits.png/320x480bb.jpg" width="185">
</div>

### Web product

**[Proveri](https://proveri.ai)** — survey and statistics SaaS

> "Surveys with publication-ready statistics, in your browser."
>
> "Build a survey, collect verified responses, and run publication-ready statistics — chi-square,
> t-tests, ANOVA, Cronbach's alpha and more — without leaving your browser."

`Python` `FastAPI` `PostgreSQL` `React` `TanStack` `Paddle` `Apple IAP` `GCP Cloud Run` `Cloudflare`
Source private.

---

### npm — 19 packages across 5 scopes

**Statistics in the browser** — the computation layer behind Proveri

[![npm](https://img.shields.io/npm/v/@winm2m/inferential-stats-js?style=flat-square&label=%40winm2m%2Finferential-stats-js&color=CB3837&logo=npm)](https://www.npmjs.com/package/@winm2m/inferential-stats-js)
[![npm](https://img.shields.io/npm/v/@winm2m/react-stats-ui?style=flat-square&label=%40winm2m%2Freact-stats-ui&color=CB3837&logo=npm)](https://www.npmjs.com/package/@winm2m/react-stats-ui)
[![npm](https://img.shields.io/npm/v/@winm2m/react-data-workspace?style=flat-square&label=%40winm2m%2Freact-data-workspace&color=CB3837&logo=npm)](https://www.npmjs.com/package/@winm2m/react-data-workspace)

> "A headless JavaScript SDK for advanced statistical analysis in the browser using WebAssembly
> (Pyodide). Performs SPSS-level inferential statistics entirely client-side with no backend
> required."

**Texo — generatable UI for LLM streams**

[![npm](https://img.shields.io/npm/v/@texo-ui/core?style=flat-square&label=%40texo-ui%2Fcore&color=CB3837&logo=npm)](https://www.npmjs.com/package/@texo-ui/core)
[![npm](https://img.shields.io/npm/v/@texo-ui/react?style=flat-square&label=%40texo-ui%2Freact&color=CB3837&logo=npm)](https://www.npmjs.com/package/@texo-ui/react)
[![npm](https://img.shields.io/npm/v/@texo-ui/standalone?style=flat-square&label=%40texo-ui%2Fstandalone&color=CB3837&logo=npm)](https://www.npmjs.com/package/@texo-ui/standalone)
[![npm](https://img.shields.io/npm/v/@texo-ui/kit?style=flat-square&label=%40texo-ui%2Fkit&color=CB3837&logo=npm)](https://www.npmjs.com/package/@texo-ui/kit)
[![npm](https://img.shields.io/npm/v/@texo-ui/data-adapter?style=flat-square&label=%40texo-ui%2Fdata-adapter&color=CB3837&logo=npm)](https://www.npmjs.com/package/@texo-ui/data-adapter)

> "Weave Text into UI. A stream-oriented Generatable UI framework for the LLM era."
>
> "Unlike Vercel's `v0` or standard generative UI tools that rely on brittle JSON or raw HTML
> generation, Texo uses a robust, human-readable syntax (Markdown Directives + YAML) to 'weave' UI
> components in real-time."

```mermaid
graph LR
    A[LLM Stream] -->|Markdown/YAML| B(Texo Parser)
    B -->|UI AST| C{Renderer}
    C -->|Web| D[React Components]
    C -->|CDN| E[Standalone Widget]
    C -->|Mobile| F[React Native — planned]
```

**Flux-Mask — client-side request encryption**

[![npm](https://img.shields.io/npm/v/@flux-mask/core?style=flat-square&label=%40flux-mask%2Fcore&color=CB3837&logo=npm)](https://www.npmjs.com/package/@flux-mask/core)
[![npm](https://img.shields.io/npm/v/@flux-mask/axios-interceptor?style=flat-square&label=%40flux-mask%2Faxios-interceptor&color=CB3837&logo=npm)](https://www.npmjs.com/package/@flux-mask/axios-interceptor)
[![npm](https://img.shields.io/npm/v/@flux-mask/fetch-wrapper?style=flat-square&label=%40flux-mask%2Ffetch-wrapper&color=CB3837&logo=npm)](https://www.npmjs.com/package/@flux-mask/fetch-wrapper)

> "Client-side libraries for Flux-Mask encryption." — core cryptography utilities, an Axios
> interceptor, and a Fetch wrapper. The server half ships as the `winm2m/fluxmask-nginx` image
> below.

**Everything else**

| Package | Version | Published | Description |
|---|---|---|---|
| [@winm2m/shadow-translate-bridge](https://www.npmjs.com/package/@winm2m/shadow-translate-bridge) | 1.5.0 | 2026-03 | "A bridge to sync Shadow DOM content with browser translation engines via Mirroring API" |
| [leanprompt-client](https://www.npmjs.com/package/leanprompt-client) | 0.1.1 | 2026-02 | "React client for LeanPrompt WebSocket communication" |
| [@proveri/survey-core](https://www.npmjs.com/package/@proveri/survey-core) | 0.0.2 | 2026-06 | Survey runtime functionality |
| [@winm2m/pretty-textarea](https://www.npmjs.com/package/@winm2m/pretty-textarea) | 1.0.5 | 2025-06 | "A WebComponent textarea implementation with custom properties and styles" |
| [@winm2m/web](https://www.npmjs.com/package/@winm2m/web) | 1.2.4 | 2024-09 | "A package for developing webbased user service" |
| [@winm2m/cfworker-base](https://www.npmjs.com/package/@winm2m/cfworker-base) | 1.1.0 | 2023-01 | "A library for creating basic CRUD endpoints for Cloudflare Workers" |
| [@winm2m/argos-api](https://www.npmjs.com/package/@winm2m/argos-api) | 0.3.1 | 2023-01 | "API for the Argos IoT Mobile Web/APP" |
| [cf-worker-mqtt-relay](https://www.npmjs.com/package/cf-worker-mqtt-relay) | 1.0.0 | 2022-12 | "A relay server for simple communication with external MQTT servers in Cloudflare Worker" |

### PyPI

[![PyPI](https://img.shields.io/pypi/v/leanprompt?style=flat-square&logo=pypi&logoColor=white&color=3775A9)](https://pypi.org/project/leanprompt/)
[![PyPI downloads](https://img.shields.io/pypi/dm/leanprompt?style=flat-square&color=3775A9)](https://pypi.org/project/leanprompt/)

> "A lightweight, engineering-first LLM framework for FastAPI featuring session-based context
> caching and reliable output validation."

13 releases, 0.1.0 → 0.4.4 · MIT

### Docker Hub

[![opencode](https://img.shields.io/docker/pulls/winm2m/opencode?style=flat-square&logo=docker&logoColor=white&label=winm2m%2Fopencode&color=2496ED)](https://hub.docker.com/r/winm2m/opencode)
[![fluxmask-nginx](https://img.shields.io/docker/pulls/winm2m/fluxmask-nginx?style=flat-square&logo=docker&logoColor=white&label=winm2m%2Ffluxmask-nginx&color=2496ED)](https://hub.docker.com/r/winm2m/fluxmask-nginx)
[![email-forward](https://img.shields.io/docker/pulls/winm2m/email-forward?style=flat-square&logo=docker&logoColor=white&label=winm2m%2Femail-forward&color=2496ED)](https://hub.docker.com/r/winm2m/email-forward)

| Image | Description |
|---|---|
| `winm2m/fluxmask-nginx` | "This Docker image provides Nginx with the Flux-Mask Lua plugin pre-installed and configured." |
| `winm2m/opencode` | "A ready-to-use Docker image for running OpenCode with all necessary models and dependencies pre-downloaded." |
| `winm2m/email-forward` | "A Docker image that forwards emails received to the specified host to another address." |

---

## 2. Public repositories — timeline

Reverse chronological. Forks of third-party projects are omitted.

### 2026

[![valet-fs](https://img.shields.io/github/stars/winm2m/valet-fs?style=flat-square&label=winm2m%2Fvalet-fs&logo=go&color=00ADD8)](https://github.com/winm2m/valet-fs) · `Go` `FUSE` `WebDAV` · `macOS` `Linux`
> "ValetFS is a Zero-Backend, P2P, in-memory virtual file system that exposes short-lived tokens
> and keys to AI agents only while a paired mobile app allows it. … No root, drivers, or FUSE are
> required — if FUSE is unavailable the daemon serves files over a loopback WebDAV endpoint and
> the local CLI instead."

[![texo-ui](https://img.shields.io/github/stars/winm2m/texo-ui?style=flat-square&label=winm2m%2Ftexo-ui&logo=typescript&color=3178C6)](https://github.com/winm2m/texo-ui) · `TypeScript` `React` · `Web`
> See Texo above.

[![inferential-stats-js](https://img.shields.io/github/stars/winm2m/inferential-stats-js?style=flat-square&label=winm2m%2Finferential-stats-js&logo=webassembly&color=654FF0)](https://github.com/winm2m/inferential-stats-js)
[![react-stats-ui](https://img.shields.io/github/stars/winm2m/react-stats-ui?style=flat-square&label=winm2m%2Freact-stats-ui&logo=react&color=61DAFB)](https://github.com/winm2m/react-stats-ui)
[![react-data-workspace](https://img.shields.io/github/stars/winm2m/react-data-workspace?style=flat-square&label=winm2m%2Freact-data-workspace&logo=react&color=61DAFB)](https://github.com/winm2m/react-data-workspace)

[![diligent-hours](https://img.shields.io/github/stars/YoungjuneKwon/diligent-hours?style=flat-square&label=diligent-hours&logo=rust&color=000000)](https://github.com/YoungjuneKwon/diligent-hours) · `Rust` `Tauri` · `Windows` `macOS`
> "A desktop timer that treats your first keyboard/mouse input of the day as the start of work,
> then shows the time remaining until the agreed workday is over and alerts you when it ends."

[![claude-voice](https://img.shields.io/github/stars/YoungjuneKwon/claude-voice?style=flat-square&label=claude-voice&logo=python&color=3776AB)](https://github.com/YoungjuneKwon/claude-voice) · `Python` · `Linux`
> "Hear what Claude Code just did, and answer it out loud — without opening the laptop. Every time
> a Claude Code turn ends, its response is summarized into a few sentences written for the ear and
> pushed to Telegram. Reply there by voice and the session picks up where it left off."

[![market-orchestrator](https://img.shields.io/github/stars/YoungjuneKwon/market-orchestrator?style=flat-square&label=market-orchestrator&logo=python&color=3776AB)](https://github.com/YoungjuneKwon/market-orchestrator) · `Python` `Node.js` `Vite` · `Linux`
> "Python + Node.js based monorepo for automated trading operations with a broker-agnostic
> architecture. … Start with Korea Investment & Securities (KIS) Open API, but keep broker
> integrations pluggable. Provide safety-first controls such as forced stop-loss sell and
> emergency stop."

[![dockerimage-winm2m-opencode](https://img.shields.io/github/stars/YoungjuneKwon/dockerimage-winm2m-opencode?style=flat-square&label=dockerimage-winm2m-opencode&logo=docker&color=2496ED)](https://github.com/YoungjuneKwon/dockerimage-winm2m-opencode) · `Docker` · `Linux`
> "A ready-to-use Docker image for running OpenCode with all necessary models and dependencies
> pre-downloaded. … Automatically built and pushed to Docker Hub on every Dockerfile update."

[![forked-semopy](https://img.shields.io/github/stars/YoungjuneKwon/forked-semopy?style=flat-square&label=forked-semopy&logo=python&color=3776AB)](https://github.com/YoungjuneKwon/forked-semopy) · `Python` — **most-starred repository**
A maintained fork of [semopy](https://bitbucket.org/herrberg/semopy):
> "semopy is an umbrella Python package that includes numerous Structural Equation Modelling (SEM)
> techniques."

[![leanprompt](https://img.shields.io/github/stars/winm2m/leanprompt?style=flat-square&label=winm2m%2Fleanprompt&logo=python&color=3776AB)](https://github.com/winm2m/leanprompt) · `Python` `FastAPI`
[![leanprompt-client](https://img.shields.io/github/stars/winm2m/leanprompt-client?style=flat-square&label=winm2m%2Fleanprompt-client&logo=react&color=61DAFB)](https://github.com/winm2m/leanprompt-client) · `TypeScript` `React`
> "A lightweight, engineering-first LLM framework for FastAPI featuring session-based context
> caching and reliable output validation." / "A React client library for LeanPrompt, providing
> seamless WebSocket synchronization and streaming hooks for AI-driven applications."

[![shadow-translate-bridge](https://img.shields.io/github/stars/YoungjuneKwon/shadow-translate-bridge?style=flat-square&label=shadow-translate-bridge&logo=typescript&color=3178C6)](https://github.com/YoungjuneKwon/shadow-translate-bridge) · `TypeScript` · `Web`
> "A lightweight bridge to sync Shadow DOM content with browser translation engines (like Google
> Translate)."

[![just-replace-http](https://img.shields.io/github/stars/YoungjuneKwon/just-replace-http?style=flat-square&label=just-replace-http&logo=googlechrome&color=4285F4)](https://github.com/YoungjuneKwon/just-replace-http) · `JavaScript` · `Chrome`
> "A Chrome extension that replaces parts of HTTP request strings with desired strings before
> sending the request. … Regex pattern matching and group references. … Provides Requestly-style
> replace functionality for free. … UI language automatically adapts to your Chrome browser
> language (English, French, Spanish, Arabic, Chinese, Russian, Korean)."

### 2025

**[flux-mask-clients](https://github.com/YoungjuneKwon/flux-mask-clients)** · 2025-12 · `TypeScript` · `Web` — see Flux-Mask above

**[froala-under-closed-shadowroot](https://github.com/YoungjuneKwon/froala-under-closed-shadowroot)** · 2025-11 · `JavaScript` · `Web`
> "Sample code for using Froala WYSIWYG editor under a closed shadow root."

**[signal-factory](https://github.com/YoungjuneKwon/signal-factory)** · 2025-11
> "Signal Factory - 상세 기획 문서."

**[product-2025-report-email-consultation](https://github.com/YoungjuneKwon/product-2025-report-email-consultation)** · 2025-10 · `Python`
> "Gmail 상담 메일을 수집하고 Excel 보고서를 생성하는 Python 프로젝트."

**[tailwind-shadcn-webcomponent](https://github.com/YoungjuneKwon/tailwind-shadcn-webcomponent)** · 2025-08 · `Web`

**[product-2025-pretty-textarea](https://github.com/YoungjuneKwon/product-2025-pretty-textarea)** · 2025-06 · `JavaScript` · `Web`
> "Textarea component which can be formatted by rule."

[![cloudflare-worker-mqtt-relay](https://img.shields.io/github/stars/YoungjuneKwon/cloudflare-worker-mqtt-relay?style=flat-square&label=cloudflare-worker-mqtt-relay&logo=cloudflare&color=F38020)](https://github.com/YoungjuneKwon/cloudflare-worker-mqtt-relay) · `JavaScript` · `Cloudflare`
> "A relay server that allows you to perform simple communication with external MQTT servers in
> Cloudflare Worker."

**[ios-native-boost-webview](https://github.com/YoungjuneKwon/ios-native-boost-webview)** · 2025-01 · `Swift` · `iOS`

### 2024 and earlier

**[android-nativeboost-webview](https://github.com/YoungjuneKwon/android-nativeboost-webview)** · 2024-12 · `Java` · `Android`
> "Webview inherated View class for enhancing performance of loading web resource."

**[product-2024-general-web](https://github.com/YoungjuneKwon/product-2024-general-web)** · 2024-09 · `JavaScript` · `Web`
> "This package is a set of features commonly used to build web-based applications. It includes
> utility functions related to JWT authentication…"

**[winm2m-docker-tunnel](https://github.com/YoungjuneKwon/winm2m-docker-tunnel)** · 2023-05 · `Docker` · `Linux`
> "A docker image for opening ssh tunnel."

**[colab_tools](https://github.com/YoungjuneKwon/colab_tools)** · 2023-04 · `Python`

**[winm2m-cfworker-base](https://github.com/YoungjuneKwon/winm2m-cfworker-base)** · 2023-01 · `JavaScript` · `Cloudflare`
> "A library for creating basic CRUD endpoints for Cloudflare Workers. It use a notion page as
> database."

**[product-2022-argos-api-js](https://github.com/YoungjuneKwon/product-2022-argos-api-js)** · 2022-11 · `JavaScript`

**[docker-sendmail-forward](https://github.com/YoungjuneKwon/docker-sendmail-forward)** · 2022-11 · `Shell` `Docker` · `Linux`
> "A Docker image that forwards emails received to the specified host to another address."

**[solidity-samples](https://github.com/YoungjuneKwon/solidity-samples)** · 2022-09 · `Solidity` · `Ethereum`
Cross-contract call samples. See [NFT Minting Platform](projects/nft-minting.md) for the
production Solidity work from the same period.

**[iotcam-android](https://github.com/YoungjuneKwon/iotcam-android)** · 2022-05 · `Java` · `Android`

**[generate-self-signed-cert](https://github.com/YoungjuneKwon/generate-self-signed-cert)** · 2021-07 · `Shell` · `Linux`

**[daily-coding](https://github.com/YoungjuneKwon/daily-coding)** · 2021-04 · `Python` `Jupyter`

**[automation_si4n](https://github.com/YoungjuneKwon/automation_si4n)** · 2021-03 · `Python`

**[dockers](https://github.com/YoungjuneKwon/dockers)** · 2021-02 · `Docker` · `Linux`

**[python-batch-resize](https://github.com/YoungjuneKwon/python-batch-resize)** · 2020-09 · `Python`
> "Resize and crop all images stored in the folder."

**[practice-math-vue](https://github.com/YoungjuneKwon/practice-math-vue)** · 2020-01 · `JavaScript` `Vue` · `Web`

**[argos-rpi-python](https://github.com/YoungjuneKwon/argos-rpi-python)** · 2019-05 · `Python` · `Raspberry Pi`
> "Python package for processing GPIO on RaspberryPI."

[![esp32-toolchain-rpi](https://img.shields.io/github/stars/YoungjuneKwon/esp32-toolchain-rpi?style=flat-square&label=esp32-toolchain-rpi&logo=espressif&color=E7352C)](https://github.com/YoungjuneKwon/esp32-toolchain-rpi) · `Shell` · `ESP32` `Raspberry Pi`
> "This is the build script and binary of the toolchain for RPi in the ESP-IDF installation guide."

**[konlpy-rest](https://github.com/YoungjuneKwon/konlpy-rest)** · 2019-04 · `Python`
> "KoNLPy를 웹 어플리케이션에서 활용할 수 있도록 만든 간단한 REST API 서비스입니다."

**[RemoteWebMouse](https://github.com/YoungjuneKwon/RemoteWebMouse)** · 2019-01

**[argos-streamer](https://github.com/YoungjuneKwon/argos-streamer)** · 2018-12 · `JavaScript` `MQTT`
> "Server application for streaming MQTT packets. Take specific topics and keep them in files for
> a certain period of time under a specific folder."

---

## 3. Deep dive

**[NFT Minting Platform](projects/nft-minting.md)** — ERC-721 launch system with Merkle-proof
allowlist and on-chain anti-bot controls (2022, client engagement). Source is private; the
document describes the engineering approach only.
`Solidity` `OpenZeppelin` `Vue 3` `Web3` · `Ethereum`
