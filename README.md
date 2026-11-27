# Awesome-OS Organization Hub (`awesome-os/.github`)

> **Organization profile, ecosystem index, and Holo `v11` entry points for [`github.com/awesome-os`](https://github.com/awesome-os).**

[![Root Portal](https://img.shields.io/badge/Portal-awesome--os.github.io-0EA5E9?style=for-the-badge)](https://awesome-os.github.io/)
[![Architecture Demos](https://img.shields.io/badge/Demos-PDP11_%C2%B7_TaskMgr_%C2%B7_3DGS-38BDF8?style=for-the-badge)](https://awesome-os.github.io/demos/)
[![Install AwesomeOS OOBE](https://img.shields.io/badge/Install-Web_OOBE_Installer-39C5CF?style=for-the-badge)](https://awesome-os.github.io/installer/)
[![Live Oversight](https://img.shields.io/badge/Telemetry-Holo_v11_Oversight-D29922?style=for-the-badge)](https://awesome-os.github.io/holo-v11/oversight.html)
[![Holo v11 CAS Index](https://img.shields.io/badge/CAS-Holo_v11_Index_JSON-F97316?style=for-the-badge)](https://awesome-os.github.io/holo-v11/cas/v11/index.json)
[![Agent Platform Hub](https://img.shields.io/badge/Live-Agent_Platform_App-2EA043?style=for-the-badge)](https://awesome-os.github.io/agent-platform/)
[![b8g.app Portal](https://img.shields.io/badge/Runtime-b8g.app_Portal-10B981?style=for-the-badge)](https://awesome-os.github.io/b8g.app/)
[![Engineering Portal](https://img.shields.io/badge/Architecture-lemanschik.com-64748B?style=for-the-badge)](https://awesome-os.github.io/lemanschik.com/)

See [`profile/README.md`](profile/README.md) for the GitHub organization overview.

---

## Flat Org Architecture (`17` Active / `129` Archived)

### 6 Canonical Monorepos

| Monorepo | Purpose |
| :--- | :--- |
| [**`awesome-os/awesome-os`**](https://github.com/awesome-os/awesome-os) | Sovereign ChromeOS-grade OS monorepo (`Holo-Linux 7.3.6` + `14.17 KB` Zig microkernel, Verified Boot, A/B rollback, Powerwash, Crostini `apt-dpkg-projector`, Fleet Host Manager, `Sectium` + `Ladybird 18/18` + `Firefox 24/24`, and `5,078` deduplicated `v11` packages) |
| [**`awesome-os/chromium-baseline`**](https://github.com/awesome-os/chromium-baseline) | Unified Chromium `160.0.8184.0` & V8 `16.0.88+` shared-library baseline (`dup_v8 = 0 B`, `components/{libv8_monolith,blink,skia,dawn,libuv,inmem-linker,angrybird,just-js}`, `browsers/{sectium,electron,brave}`, `runtimes/{node,deno,bun-neon}`, live compiled native release [`v11-chromium-baseline-latest`](https://github.com/awesome-os/chromium-baseline/releases/tag/v11-chromium-baseline-latest)) |
| [**`awesome-os/agent-platform`**](https://github.com/awesome-os/agent-platform) | Sovereign AI & Autonomous Agent Platform (LLM & LoRA Studio, Model Garden, `ZER0Q`, `AtlasKV`, Brain RAG, Model Armor, `Colibri` / `llama.cpp` / `vLLM`, A2A / MCP / A2UI / x402) |
| [**`awesome-os/t2linux-baseline`**](https://github.com/awesome-os/t2linux-baseline) | T2 SDE Baseline Edition & 2-tier selectable graphics OS (`~31 MB` base OS + opt-in Wayland + default rootless `Xwayland` + `5,078` `v11` packages + frozen `packages-legacy`) |
| [**`awesome-os/devtools`**](https://github.com/awesome-os/devtools) | Unified DevTools Monorepo (`ide/{code-oss,theia,b8g-ide}`, VS Code / Open VSX extensions, Game Engines `b8g-game-engine` / `asymmetric-hunt` / `godot` / `blender`, native C11 dynamic launchers [`v11-devtools-launchers-latest`](https://github.com/awesome-os/devtools/releases/tag/v11-devtools-launchers-latest), 4DGS research) |
| [**`awesome-os/wordpress-ecosystem`**](https://github.com/awesome-os/wordpress-ecosystem) | Sovereign WordPress core, WooCommerce, and enterprise PHP/WASI plugin monorepo |

---

### 7 Control-Plane, CAS, Delivery & Demo Hubs

| Hub | Purpose |
| :--- | :--- |
| [**`awesome-os/holo-v11`**](https://github.com/awesome-os/holo-v11) | Global Auditable Holo `v11` CAS Registry (`B8G_ABI_MAGIC_V3 = 0x33564742`, Planetary Warm CAS, `68/68` tracked upstream libs, `index/holo-compiler-lockfile.json`, `index/cas-v11-global-manifest.json`, honest compiled-vs-virtual `materialization` telemetry, `CAS Q-Self` fixed-point proofs) |
| [**`awesome-os/maintenance-workflows`**](https://github.com/awesome-os/maintenance-workflows) | Centralized zero-dependency Node 24/26 **`holo-ci@v1`** (`reusable-holo-ci.yml@v1`, `reusable-holo-e2e.yml@v1`), 9-ecosystem `holo-ci lock-compat` (`npm`, `cargo`, `uv`, `go`, `vcpkg`, `winget`, `apt`, `composer`, `rubygems`), 5-OS Zig C11 release workflows, VSIX / Open VSX releases, and `holo-ci.receipt.v1` telemetry |
| [**`awesome-os/upstream-mirrors`**](https://github.com/awesome-os/upstream-mirrors) | Cross-compiled 5-OS + WASI shared native library artifacts ([`v11-max-5os-latest`](https://github.com/awesome-os/upstream-mirrors/releases/tag/v11-max-5os-latest)) feeding Planetary Warm CAS |
| [**`awesome-os/dockerimages`**](https://github.com/awesome-os/dockerimages) | Zero-Alpine `FROM scratch` `t2linux` & Node 27 `holo-node` multi-arch OCI container suite (`9` base + `16` stack images via `1:1` CAS shell pipe build + anonymous [`v11-oci-latest`](https://github.com/awesome-os/dockerimages/releases/tag/v11-oci-latest)) |
| [**`awesome-os/installer`**](https://github.com/awesome-os/installer) | Sovereign Web OOBE & CLI installer (`https://awesome-os.github.io/installer/` · `curl -fsSL https://raw.githubusercontent.com/awesome-os/installer/main/start-here.sh \| sh`) with zero-checkout Clean-Box Stranger E2E verification |
| [**`awesome-os/deployment`**](https://github.com/awesome-os/deployment) | Infrastructure-as-code, edge routing, and sovereign fleet deployment manifests |
| [**`awesome-os/demos`**](https://github.com/awesome-os/demos) | Sparse `--no-cone` architecture demo monorepo (`arch/pdp11/`, `arch/task-manager/`, `arch/graphics/` — live at `https://awesome-os.github.io/demos/`) |

---

### 4 Org & `github.io` Static Web Anchors

| Anchor | Purpose |
| :--- | :--- |
| [**`awesome-os/.github`**](https://github.com/awesome-os/.github) | Org profile, community health files, and ecosystem architecture hub |
| [**`awesome-os/awesome-os.github.io`**](https://github.com/awesome-os/awesome-os.github.io) | Root public portal (`https://awesome-os.github.io/` · `/blog/`, `/book/`, `/evidence/`, `/kids/`, `/b8g-app/`) |
| [**`awesome-os/b8g.app`**](https://github.com/awesome-os/b8g.app) | B8G universal runtime application portal (`https://awesome-os.github.io/b8g.app/`) |
| [**`awesome-os/lemanschik.com`**](https://github.com/awesome-os/lemanschik.com) | Sovereign engineering & architecture portal (`https://awesome-os.github.io/lemanschik.com/`) |

> **Archive Preservation Guarantee:** All `37` absorbed companion repositories remain preserved read-only (`129` total archived repositories) with 100% of their published GitHub Releases indexed in `awesome-os/holo-v11` via `CONSOLIDATED_ARCHIVE_ALLOWLIST`.

---

## Live Production Links

- **Root Public Portal:** [https://awesome-os.github.io/](https://awesome-os.github.io/) (`/blog/`, `/book/`, `/evidence/`, `/kids/`, `/b8g-app/`)
- **Sparse Architecture Demos (`arch/pdp11/`, `arch/task-manager/`, `arch/graphics/`):** [https://awesome-os.github.io/demos/](https://awesome-os.github.io/demos/)
- **Install Awesome-OS (Web OOBE & Clean-Box Stranger E2E):** [https://awesome-os.github.io/installer/](https://awesome-os.github.io/installer/) (zero-checkout live-binary Clean-Box Stranger E2E verified in [`awesome-os/installer`](https://github.com/awesome-os/installer))
- **Live Holo `v11` Oversight Telemetry (`68/68` upstream libs):** [https://awesome-os.github.io/holo-v11/oversight.html](https://awesome-os.github.io/holo-v11/oversight.html)
- **Holo `v11` CAS Index (`index.json`):** [https://awesome-os.github.io/holo-v11/cas/v11/index.json](https://awesome-os.github.io/holo-v11/cas/v11/index.json)
- **Unified Agent Platform Control Center:** [https://awesome-os.github.io/agent-platform/](https://awesome-os.github.io/agent-platform/)
- **Sovereign LLM & LoRA Studio:** [https://awesome-os.github.io/agent-platform/llm-studio.html](https://awesome-os.github.io/agent-platform/llm-studio.html)
- **B8G Universal Runtime Application Portal (`awesome-os/b8g.app`):** [https://awesome-os.github.io/b8g.app/](https://awesome-os.github.io/b8g.app/)
- **Sovereign Engineering & Architecture Portal (`awesome-os/lemanschik.com`):** [https://awesome-os.github.io/lemanschik.com/](https://awesome-os.github.io/lemanschik.com/)
