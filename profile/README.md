# Awesome-OS & Sectium

> **A sovereign, ChromeOS-grade, content-addressed operating system, runtime, browser, DevTools, and AI ecosystem — built natively with `holo-compiler` (`< 1 s`, zero WSL), zero duplicated monoliths (`dup_v8 = 0 B`), and one unified SHA-512 + Ed25519 Holo `v11` CAS ([`awesome-os/holo-v11`](https://github.com/awesome-os/holo-v11)).**

[![Install AwesomeOS OOBE](https://img.shields.io/badge/Install-Web_OOBE_Installer-39C5CF?style=for-the-badge)](https://awesome-os.github.io/installer/)
[![Live Oversight](https://img.shields.io/badge/Telemetry-Holo_v11_Oversight-D29922?style=for-the-badge)](https://awesome-os.github.io/holo-v11/oversight.html)
[![Agent Platform Hub](https://img.shields.io/badge/Live-Agent_Platform_App-2EA043?style=for-the-badge)](https://awesome-os.github.io/agent-platform/)
[![LLM & LoRA Studio](https://img.shields.io/badge/Studio-LLM_%26_LoRA_5--Tab-A78BFA?style=for-the-badge)](https://awesome-os.github.io/agent-platform/llm-studio.html)

---

## Flat Org Architecture (`16` Active / `129` Archived)

### 6 Canonical Monorepos

| Monorepo | Scope & Consolidated Stack |
| :--- | :--- |
| [**`awesome-os/awesome-os`**](https://github.com/awesome-os/awesome-os) | Core OS (`Holo-Linux 7.3.6` + `14.17 KB` Zig microkernel), Limine / iPXE Verified Boot, A/B atomic rollback, 1-Click Powerwash, Crostini `AF_VSOCK` + `apt-dpkg-projector`, Fleet Host Manager, `Sectium` + `Ladybird (18/18)` + `Firefox (24/24)` browser engines, and `5,078` deduplicated `v11` packages |
| [**`awesome-os/chromium-baseline`**](https://github.com/awesome-os/chromium-baseline) | Unified Chromium `160.0.8184.0` & V8 `16.0.88+` shared-library baseline (`dup_v8 = 0 B`) — `components/{libv8_monolith,blink,skia,dawn,libuv,inmem-linker,angrybird,just-js}`, `browsers/{sectium,electron,brave}`, `runtimes/{node,deno,bun-neon}`, and live compiled native release [`v11-chromium-baseline-latest`](https://github.com/awesome-os/chromium-baseline/releases/tag/v11-chromium-baseline-latest) |
| [**`awesome-os/agent-platform`**](https://github.com/awesome-os/agent-platform) | Sovereign AI & Autonomous Agent Platform — LLM & LoRA Studio, Model Garden (`Inkling 2 Mini`, `B8G Xenon 1B`, `LittleBit`, `Micro-MoE`, `SpinWave`, `LumiBERT`), `ZER0Q`, `AtlasKV`, Brain RAG, Model Armor, `Colibri` / `llama.cpp` / `vLLM`, and A2A / MCP / A2UI / x402 |
| [**`awesome-os/t2linux-baseline`**](https://github.com/awesome-os/t2linux-baseline) | T2 SDE Baseline Edition & 2-tier selectable graphics OS (`~31 MB` base OS with `/dev/fb0` + `kitty-ink` + `ttyS0`, opt-in Wayland + default rootless `Xwayland`, `5,078` `v11` packages, and frozen `packages-legacy`) |
| [**`awesome-os/devtools`**](https://github.com/awesome-os/devtools) | Unified DevTools Monorepo — IDEs (`ide/code-oss`, `ide/theia`, `ide/b8g-ide`), VS Code / Open VSX extensions, Game Engines (`b8g-game-engine`, `asymmetric-hunt`, `godot`, `blender`), native C11 dynamic launchers (`holo-devtools-launcher` · [`v11-devtools-launchers-latest`](https://github.com/awesome-os/devtools/releases/tag/v11-devtools-launchers-latest)), and 4DGS research |
| [**`awesome-os/wordpress-ecosystem`**](https://github.com/awesome-os/wordpress-ecosystem) | Sovereign WordPress core, WooCommerce, and enterprise PHP/WASI plugin monorepo |

---

### 6 Control-Plane, CAS & Delivery Hubs

| Hub | Role |
| :--- | :--- |
| [**`awesome-os/holo-v11`**](https://github.com/awesome-os/holo-v11) | Global Auditable Holo `v11` CAS Registry (`B8G_ABI_MAGIC_V3 = 0x33564742`, Planetary Warm CAS, `68/68` tracked upstream libs, honest compiled-vs-virtual `materialization` telemetry) — Git-versioned `index/holo-compiler-lockfile.json`, `index/cas-v11-global-manifest.json`, and `CAS Q-Self` cryptographic fixed-point proofs |
| [**`awesome-os/maintenance-workflows`**](https://github.com/awesome-os/maintenance-workflows) | Centralized zero-dependency Node 24/26 **`holo-ci@v1`** (`reusable-holo-ci.yml@v1` + `reusable-holo-e2e.yml@v1`), 7-ecosystem `holo-ci lock-compat` (`npm`, `cargo`, `uv`, `go`, `vcpkg`, `winget`, `apt`), 5-OS Zig C11 matrix builds (`reusable-5os-release.yml`), VSIX / Open VSX releases, and `holo-ci.receipt.v1` telemetry |
| [**`awesome-os/upstream-mirrors`**](https://github.com/awesome-os/upstream-mirrors) | Cross-compiled 5-OS + WASI shared native library artifacts ([`v11-max-5os-latest`](https://github.com/awesome-os/upstream-mirrors/releases/tag/v11-max-5os-latest)) indexed in Planetary Warm CAS |
| [**`awesome-os/dockerimages`**](https://github.com/awesome-os/dockerimages) | Zero-Alpine `FROM scratch` `t2linux` & Node 27 `holo-node` multi-arch OCI container suite (`8` images in [`v11-oci-latest`](https://github.com/awesome-os/dockerimages/releases/tag/v11-oci-latest)) |
| [**`awesome-os/installer`**](https://github.com/awesome-os/installer) | Web OOBE & CLI sovereign installer with zero-checkout live-binary Clean-Box Stranger E2E verification |
| [**`awesome-os/deployment`**](https://github.com/awesome-os/deployment) | Infrastructure-as-code, DNS, edge routing, and sovereign fleet deployment manifests |

---

### 4 Org & Static Web Anchors

| Anchor | Role |
| :--- | :--- |
| [**`awesome-os/.github`**](https://github.com/awesome-os/.github) | Organization profile, community health files, and ecosystem architecture hub |
| [**`awesome-os/awesome-os.github.io`**](https://github.com/awesome-os/awesome-os.github.io) | Public web presence (`https://awesome-os.github.io/`) & Oversight / Web OOBE static delivery |
| [**`awesome-os/b8g.app`**](https://github.com/awesome-os/b8g.app) | B8G universal runtime application portal (`https://awesome-os.github.io/b8g-app/`) |
| [**`awesome-os/lemanschik.com`**](https://github.com/awesome-os/lemanschik.com) | Sovereign engineering & architecture portal (`https://lemanschik.com`) |

> **Archive Preservation Guarantee:** All `37` absorbed companion repositories remain preserved read-only (`129` total archived repositories) with 100% of their published GitHub Releases indexed in `awesome-os/holo-v11` via `CONSOLIDATED_ARCHIVE_ALLOWLIST`.

---

## Live Production Apps & Installers

- **Web OOBE Installer & Clean-Box Stranger E2E (`https://awesome-os.github.io/installer/`):** [https://awesome-os.github.io/installer/](https://awesome-os.github.io/installer/) (zero-checkout live-binary Clean-Box Stranger E2E verified in [`awesome-os/installer`](https://github.com/awesome-os/installer))
- **Live Holo `v11` Oversight Telemetry (`68/68` tracked upstream libs, `0` drifted):** [https://awesome-os.github.io/holo-v11/oversight.html](https://awesome-os.github.io/holo-v11/oversight.html)
- **Unified Agent Platform Control Center:** [https://awesome-os.github.io/agent-platform/](https://awesome-os.github.io/agent-platform/)
- **Sovereign LLM & LoRA Studio:** [https://awesome-os.github.io/agent-platform/llm-studio.html](https://awesome-os.github.io/agent-platform/llm-studio.html)
