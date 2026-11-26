# Awesome-OS & Sectium

> **A sovereign, ChromeOS-grade, content-addressed operating system, runtime, browser, DevTools, and AI ecosystem — built natively with `holo-compiler` (`< 1 s`, zero WSL), zero duplicated monoliths (`dup_v8 = 0 B`), and one unified SHA-512 + Ed25519 Holo `v11` CAS ([`awesome-os/holo-v11`](https://github.com/awesome-os/holo-v11)).**

[![Install AwesomeOS OOBE](https://img.shields.io/badge/Install-Web_OOBE_Installer-39C5CF?style=for-the-badge)](https://awesome-os.com/install/)
[![Live Oversight](https://img.shields.io/badge/Telemetry-Holo_v11_Oversight-D29922?style=for-the-badge)](https://b8g.dev/awesome-os/apps/oversight.html)
[![Agent Platform Hub](https://img.shields.io/badge/Live-Agent_Platform_App-2EA043?style=for-the-badge)](https://b8g.dev/awesome-os/apps/agent-platform.html)
[![LLM & LoRA Studio](https://img.shields.io/badge/Studio-LLM_%26_LoRA_5--Tab-A78BFA?style=for-the-badge)](https://b8g.dev/awesome-os/apps/llm-studio.html)

---

## 5 Canonical Monorepos

| Monorepo | Scope & Consolidated Stack |
| :--- | :--- |
| [**`awesome-os/awesome-os`**](https://github.com/awesome-os/awesome-os) | Core OS (`Holo-Linux 7.3.6` + `14.17 KB` Zig microkernel), Limine / iPXE Verified Boot, A/B atomic rollback, 1-Click Powerwash, Crostini `AF_VSOCK` + `apt-dpkg-projector`, Fleet Host Manager, `Sectium` + `Ladybird (18/18)` + `Firefox (24/24)` browser engines, and `5,075` deduplicated `v11` packages |
| [**`awesome-os/chromium-baseline`**](https://github.com/awesome-os/chromium-baseline) | Unified Chromium `160.0.8184.0` & V8 `16.0.88+` shared-library baseline (`dup_v8 = 0 B`) — `components/{libv8_monolith,blink,skia,dawn,libuv,inmem-linker,angrybird,just-js}`, `browsers/{sectium,electron,brave}`, `runtimes/{node,deno,bun-neon}`, and live compiled native release [`v11-chromium-baseline-latest`](https://github.com/awesome-os/chromium-baseline/releases/tag/v11-chromium-baseline-latest) |
| [**`awesome-os/agent-platform`**](https://github.com/awesome-os/agent-platform) | Sovereign AI & Autonomous Agent Platform — LLM & LoRA Studio, Model Garden (`Inkling 2 Mini`, `B8G Xenon 1B`, `LittleBit`, `Micro-MoE`, `SpinWave`, `LumiBERT`), `ZER0Q`, `AtlasKV`, Brain RAG, Model Armor, `Colibri` / `llama.cpp` / `vLLM`, and A2A / MCP / A2UI / x402 |
| [**`awesome-os/t2linux-baseline`**](https://github.com/awesome-os/t2linux-baseline) | T2 SDE Baseline Edition & 2-tier selectable graphics OS (`~31 MB` base OS with `/dev/fb0` + `kitty-ink` + `ttyS0`, opt-in Wayland + default rootless `Xwayland`, `5,075` `v11` packages, and frozen `packages-legacy`) |
| [**`awesome-os/devtools`**](https://github.com/awesome-os/devtools) | Unified DevTools Monorepo — IDEs (`ide/code-oss`, `ide/theia`, `ide/b8g-ide`), VS Code / Open VSX extensions, Game Engines (`b8g-game-engine`, `asymmetric-hunt`, `godot`, `blender`), native C11 dynamic launchers (`holo-devtools-launcher` · [`v11-devtools-launchers-latest`](https://github.com/awesome-os/devtools/releases/tag/v11-devtools-launchers-latest)), and 4DGS research |

---

## 2 Holo Control-Plane Hubs

| Control-Plane Hub | Role |
| :--- | :--- |
| [**`awesome-os/holo-v11`**](https://github.com/awesome-os/holo-v11) | Global Auditable Holo `v11` CAS Registry (`B8G_ABI_MAGIC_V3 = 0x33564742`, Planetary Warm CAS: `60` repos / `413` assets / `402` unique SHA-512 blobs / `1,454 MB` raw, `19/22` ecosystems at `100%`) — Git-versioned `index/holo-compiler-lockfile.json`, `index/cas-v11-global-manifest.json`, and `CAS Q-Self` cryptographic fixed-point proofs |
| [**`awesome-os/maintenance-workflows`**](https://github.com/awesome-os/maintenance-workflows) | Centralized zero-dependency Node 24/26 **`holo-ci@v1`** (`reusable-holo-ci.yml@v1`, `23` active repos onboarded), 7-ecosystem `holo-ci lock-compat` (`npm`, `cargo`, `uv`, `go`, `vcpkg`, `winget`, `apt`), 5-OS Zig C11 matrix builds (`reusable-5os-release.yml`), VSIX / Open VSX releases, and `holo-ci.receipt.v1` telemetry |

---

## Live Production Apps & Installers

- **Web OOBE Installer & Clean-Box Stranger E2E (`https://awesome-os.com/install/`):** [https://awesome-os.com/install/](https://awesome-os.com/install/) (zero-checkout live-binary Clean-Box Stranger E2E verified in [`awesome-os/installer`](https://github.com/awesome-os/installer))
- **Live Holo `v11` Oversight Telemetry (`60/60` tracked upstream libs, `0` drifted, `19/22` ecosystems at `100%`):** [https://b8g.dev/awesome-os/apps/oversight.html](https://b8g.dev/awesome-os/apps/oversight.html)
- **Unified Agent Platform Control Center:** [https://b8g.dev/awesome-os/apps/agent-platform.html](https://b8g.dev/awesome-os/apps/agent-platform.html)
- **Sovereign LLM & LoRA Studio:** [https://b8g.dev/awesome-os/apps/llm-studio.html](https://b8g.dev/awesome-os/apps/llm-studio.html)

---

## Active Companion Repositories

| Category | Repositories |
| :--- | :--- |
| **Holo Toolchain & SDK** | [**holo-compiler**](https://github.com/awesome-os/holo-compiler) · [**holo-pm**](https://github.com/awesome-os/holo-pm) · [**holo-sdk**](https://github.com/awesome-os/holo-sdk) · [**upstream-mirrors**](https://github.com/awesome-os/upstream-mirrors) · [**dockerimages**](https://github.com/awesome-os/dockerimages) |
| **Browsers, Desktop & Wayland** | [**sectium-browser**](https://github.com/awesome-os/sectium-browser) · [**desktop**](https://github.com/awesome-os/desktop) · [**desktop-omarchy**](https://github.com/awesome-os/desktop-omarchy) · [**explorer**](https://github.com/awesome-os/explorer) · [**noctalia**](https://github.com/awesome-os/noctalia) · [**chonkstep**](https://github.com/awesome-os/chonkstep) |
| **Languages, Runtimes & Core** | [**typescript**](https://github.com/awesome-os/typescript) · [**lo**](https://github.com/awesome-os/lo) · [**ts-morph**](https://github.com/awesome-os/ts-morph) · [**ts-sema**](https://github.com/awesome-os/ts-sema) · [**coreutils**](https://github.com/awesome-os/coreutils) · [**cargo**](https://github.com/awesome-os/cargo) · [**go-lang**](https://github.com/awesome-os/go-lang) · [**dart**](https://github.com/awesome-os/dart) · [**uv**](https://github.com/awesome-os/uv) |
| **Live Sites** | [**awesome-os.com**](https://awesome-os.com) ([`awesome-os.github.io`](https://github.com/awesome-os/awesome-os.github.io)) · [**b8g.app**](https://b8g.app) ([`b8g.app`](https://github.com/awesome-os/b8g.app)) |
