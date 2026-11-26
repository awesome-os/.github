# Awesome-OS Organization Hub (`awesome-os/.github`)

> **Organization profile, ecosystem index, and Holo `v11` entry points for [`github.com/awesome-os`](https://github.com/awesome-os).**

See [`profile/README.md`](profile/README.md) for the GitHub organization overview.

---

## 5 Canonical Monorepos

| Monorepo | Purpose |
| :--- | :--- |
| [**`awesome-os/awesome-os`**](https://github.com/awesome-os/awesome-os) | Sovereign ChromeOS-grade OS monorepo (`Holo-Linux 7.3.6` + `14.17 KB` Zig microkernel, Verified Boot, A/B rollback, Powerwash, Crostini `apt-dpkg-projector`, Fleet Host Manager, `Sectium` + `Ladybird 18/18` + `Firefox 24/24`, and `5,075` deduplicated `v11` packages) |
| [**`awesome-os/chromium-baseline`**](https://github.com/awesome-os/chromium-baseline) | Unified Chromium `160.0.8184.0` & V8 `16.0.88+` shared-library baseline (`dup_v8 = 0 B`, `components/{libv8_monolith,blink,skia,dawn,libuv,inmem-linker,angrybird,just-js}`, `browsers/{sectium,electron,brave}`, `runtimes/{node,deno,bun-neon}`, live compiled native release [`v11-chromium-baseline-latest`](https://github.com/awesome-os/chromium-baseline/releases/tag/v11-chromium-baseline-latest)) |
| [**`awesome-os/agent-platform`**](https://github.com/awesome-os/agent-platform) | Sovereign AI & Autonomous Agent Platform (LLM & LoRA Studio, Model Garden, `ZER0Q`, `AtlasKV`, Brain RAG, Model Armor, `Colibri` / `llama.cpp` / `vLLM`, A2A / MCP / A2UI / x402) |
| [**`awesome-os/t2linux-baseline`**](https://github.com/awesome-os/t2linux-baseline) | T2 SDE Baseline Edition & 2-tier selectable graphics OS (`~31 MB` base OS + opt-in Wayland + default rootless `Xwayland` + `5,075` `v11` packages + frozen `packages-legacy`) |
| [**`awesome-os/devtools`**](https://github.com/awesome-os/devtools) | Unified DevTools Monorepo (`ide/{code-oss,theia,b8g-ide}`, VS Code / Open VSX extensions, Game Engines `b8g-game-engine` / `asymmetric-hunt` / `godot` / `blender`, native C11 dynamic launchers [`v11-devtools-launchers-latest`](https://github.com/awesome-os/devtools/releases/tag/v11-devtools-launchers-latest), 4DGS research) |

---

## 2 Holo Control-Plane Hubs

| Hub | Purpose |
| :--- | :--- |
| [**`awesome-os/holo-v11`**](https://github.com/awesome-os/holo-v11) | Global Auditable Holo `v11` CAS Registry (`B8G_ABI_MAGIC_V3 = 0x33564742`, Planetary Warm CAS: `60` repos / `413` assets / `1,454 MB` raw, `60/60` tracked upstream libs with `0` drifted, `19/22` ecosystems at `100%`, `index/holo-compiler-lockfile.json`, `index/cas-v11-global-manifest.json`, `CAS Q-Self` fixed-point proofs) |
| [**`awesome-os/maintenance-workflows`**](https://github.com/awesome-os/maintenance-workflows) | Centralized zero-dependency Node 24/26 **`holo-ci@v1`** (`reusable-holo-ci.yml@v1`, `23` active repos onboarded), 7-ecosystem `holo-ci lock-compat` (`npm`, `cargo`, `uv`, `go`, `vcpkg`, `winget`, `apt`), 5-OS Zig C11 release workflows, VSIX / Open VSX releases, and `holo-ci.receipt.v1` telemetry |

---

## Live Production Links

- **Install Awesome-OS (Web OOBE & Clean-Box Stranger E2E):** [https://awesome-os.com/install/](https://awesome-os.com/install/) (zero-checkout live-binary Clean-Box Stranger E2E verified in [`awesome-os/installer`](https://github.com/awesome-os/installer))
- **Live Holo `v11` Oversight Telemetry (`60/60` upstream libs, `19/22` ecosystems at `100%`):** [https://b8g.dev/awesome-os/apps/oversight.html](https://b8g.dev/awesome-os/apps/oversight.html)
- **Unified Agent Platform Control Center:** [https://b8g.dev/awesome-os/apps/agent-platform.html](https://b8g.dev/awesome-os/apps/agent-platform.html)
- **Sovereign LLM & LoRA Studio:** [https://b8g.dev/awesome-os/apps/llm-studio.html](https://b8g.dev/awesome-os/apps/llm-studio.html)
