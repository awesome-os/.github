# Awesome-OS & Sectium

> **A sovereign, content-addressed operating system, runtime, and browser/IDE ecosystem — built natively with `holo-compiler`, zero duplicated monoliths, and one canonical $O(1)$ Ghost CAS ([`awesome-os/b8g-ghost @ cas-v1`](https://github.com/awesome-os/b8g-ghost)).**

**Measured live on Windows 11:** **`Awesome-OS Code - OSS 1.147.0`** (`477 MB`) + **`Sectium Browser`** (`110 MB`) side by side in **`587 MB` total RAM** — **`7.7×` less RAM than one `4.5 GB` VS Code window**, launched from **`~118 KB`** native Lumi Hydration Splash `.exe` binaries sharing ONE `b8g-ghost` CAS runtime (`0 B` duplicated Electron).

---

## Collapsed 4-Layer Architecture

1. **Sectium & Desktop Appliances** — `~118 KB` native Lumi Hydration Splash launchers ([`sectium-browser`](https://github.com/awesome-os/sectium-browser), [`code-oss`](https://github.com/awesome-os/code-oss), [`theia`](https://github.com/awesome-os/theia), [`brave`](https://github.com/awesome-os/brave), [`blender`](https://github.com/awesome-os/blender), [`obs`](https://github.com/awesome-os/obs), [`godot`](https://github.com/awesome-os/godot), [`pinokio`](https://github.com/awesome-os/pinokio)) + pure-art Sectium Canvas (`0` closed Google/MS DLLs).
2. **Sectium Cloud Control Plane** — `5.0 KB` C11 `B8G_ABI_MAGIC_V3` central discovery `initramfs`, 1-way `WoL` warm-RAM resume, and Keep-Last-5 `RollingReleaseManifest` rollbacks.
3. **Host Device & `b8g-ghost` CAS** — Dual `command`/`display` NDJSON pipe (`\\.\pipe\sectium-dev`), `B8G_ARENA_V1` 64-byte zero-copy IPC, and **`156+` verified `cas-v1` blobs** (`awesome-os/b8g-ghost`).
4. **Polyglot Runtimes & T2 OS Family** — Zero-WSL 5-OS `holo-compiler`, Shared V8 (`dup_v8=0 B`), Wave 2 TypeScript `6.0.3` (`14.3×` faster Zero-AST CAS), `.NET 11`, `PowerShell 7.7`, `Node 27`, and bootable **T2Linux / T2XNU / T2Desktop**.

---

## Flagship Repositories & Live Sites

| Category | Repositories |
| :--- | :--- |
| **Core & CAS** | [**awesome-os**](https://github.com/awesome-os/awesome-os) · [**b8g-ghost**](https://github.com/awesome-os/b8g-ghost) (`156+` `cas-v1` entries) · [**upstream-mirrors**](https://github.com/awesome-os/upstream-mirrors) (`26` mirrors, `35/35` 5-OS shards) · [**chromium.googlesource.com**](https://github.com/awesome-os/chromium.googlesource.com) |
| **Operating Systems & OCI** | [**t2linux**](https://github.com/awesome-os/t2linux) (UEFI/BIOS ISO & QCOW2) · [**t2xnu**](https://github.com/awesome-os/t2xnu) (ARM64 Linux 7.0 + `xnulinux`) · [**t2desktop**](https://github.com/awesome-os/t2desktop) (Omarchy MIT + Lumi Chromatic) · [**dockerimages**](https://github.com/awesome-os/dockerimages) (`2.1 MB` `FROM scratch` multi-arch OCI) |
| **Browsers & Desktop Appliances** | [**sectium-browser**](https://github.com/awesome-os/sectium-browser) · [**code-oss**](https://github.com/awesome-os/code-oss) · [**theia**](https://github.com/awesome-os/theia) · [**brave**](https://github.com/awesome-os/brave) · [**blender**](https://github.com/awesome-os/blender) · [**obs**](https://github.com/awesome-os/obs) · [**godot**](https://github.com/awesome-os/godot) · [**pinokio**](https://github.com/awesome-os/pinokio) · [**electron**](https://github.com/awesome-os/electron) · [**sectium-electron**](https://github.com/awesome-os/sectium-electron) |
| **Unified IDE Extensions** | [**stealifylang-vscode**](https://github.com/awesome-os/stealifylang-vscode) (`stealify-lint` + rules + Wave 2 TS `6.0.3`) · [**unreal-vscode**](https://github.com/awesome-os/unreal-vscode) · [**godot-vscode**](https://github.com/awesome-os/godot-vscode) · [**blender-vscode**](https://github.com/awesome-os/blender-vscode) · [**obs-vscode**](https://github.com/awesome-os/obs-vscode) |
| **Runtimes, Compilers & Shards** | [**typescript**](https://github.com/awesome-os/typescript) (`6.0.3` Wave 1+2) · [**node**](https://github.com/awesome-os/node) (`v27`) · [**dotnet**](https://github.com/awesome-os/dotnet) (`11.0.100`) · [**powershell**](https://github.com/awesome-os/powershell) (`7.7.0`) · [**qt**](https://github.com/awesome-os/qt) (`6.10.3`) · [**skia**](https://github.com/awesome-os/skia) · [**dawn**](https://github.com/awesome-os/dawn) · [**blink**](https://github.com/awesome-os/blink) · [**libv8_monolith**](https://github.com/awesome-os/libv8_monolith) · [**lo**](https://github.com/awesome-os/lo) · [**just-js**](https://github.com/awesome-os/just-js) |
| **Language CAS Adapters** | [**ghost-py**](https://github.com/awesome-os/ghost-py) · [**ghost-jvm**](https://github.com/awesome-os/ghost-jvm) · [**ghost-cpp**](https://github.com/awesome-os/ghost-cpp) · [**ghost-100**](https://github.com/awesome-os/ghost-100) · [**sectium-es**](https://github.com/awesome-os/sectium-es) · [**sectium-jvm**](https://github.com/awesome-os/sectium-jvm) |
| **Live Sites** | [**awesome-os.com**](https://awesome-os.com) ([`awesome-os.github.io`](https://github.com/awesome-os/awesome-os.github.io)) · [**b8g.app**](https://b8g.app) ([`b8g.app`](https://github.com/awesome-os/b8g.app)) |

---

## Documentation
- [Master Architecture & Ecosystem Overview](https://github.com/awesome-os/awesome-os/blob/main/README.md)
- [Holistic 5-Ecosystem Efficiency, Cost & Energy Analysis](https://github.com/awesome-os/awesome-os/blob/main/docs/HOLISTIC-ECOSYSTEM-EFFICIENCY-ANALYSIS.md)
- [Sovereign LLM, Embeddings, Unsloth LoRA & Colab Mesh Guide](https://github.com/awesome-os/awesome-os/blob/main/docs/SOVEREIGN-LLM-STACK-GUIDE.md)
- [Mental-Model & Tooling Cheatsheet](https://github.com/awesome-os/awesome-os/blob/main/docs/AWESOME-OS-CHEATSHEET.md)
