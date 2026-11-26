# Contributing to Awesome-OS

Thank you for contributing to the Awesome-OS ecosystem. Our workflow is inspired by Chromium's engineering discipline: every non-trivial change is tracked, verified through hermetic automation, and landed with clean linear history.

## 1. Issue-First Workflow

- **Open or reference a tracking Issue** in [`awesome-os/awesome-os`](https://github.com/awesome-os/awesome-os/issues) before starting non-trivial work (features, architectural RFCs, native materializations, or multi-repo changes).
- Choose the appropriate Issue Form (`Bug Report`, `RFC / Design Doc`, or `Materialize Upstream Library`).
- Reference the tracking issue in every commit and pull request using the `Bug:` trailer.

## 2. Branch, PR & Linear History

- Work on a dedicated topic branch off `main` (never push unreviewed changes directly to `main`).
- Keep **linear commit history** (rebase or squash onto `main`; avoid merge commits).
- All required CI gates must pass before merge:
  - `holo-ci verify` (via `awesome-os/maintenance-workflows` `reusable-holo-ci.yml@v1`)
  - `Holo-E2E` (via `reusable-holo-e2e.yml@v1`)
  - Atomic `bin/` triplet parity (`b8g-bin-parity verify`) and documentation/link checks where applicable.

## 3. Commit Trailer Standard

Include structured Chromium-style trailers at the bottom of commit messages and PR descriptions:

```text
Bug: awesome-os/awesome-os#<id>
Materializes: <pkg>@<ver>
Verified-By: holo-ci@v1
```

- `Bug:` *(required for non-trivial changes)* — Links the canonical tracking issue in `awesome-os/awesome-os`.
- `Materializes:` *(when adding or updating compiled CAS artifacts)* — Exact upstream package and version materialized into Holo `v11`.
- `Verified-By:` — Verification gate or runner receipt confirming the change (e.g., `holo-ci@v1`).

## 4. Non-Negotiable Workspace Invariants

All contributions across the 16 active repositories must uphold these invariants:

1. **Hermetic `bin/` Shims:** Route tool and runtime invocations through repository `bin/` atomic `(posix, .cmd, .ps1)` triplets, `@awesome-os/bin-shim`, or `stealifylang`. Never invoke un-shimmed ambient host binaries or leave orphaned wrappers.
2. **Zero `npx`:** Never use `npx` in scripts, docs, or workflows. Always use `pnx`.
3. **Zero Local HTTP IPC (`B8G016`):** Local OS, VM, and daemon IPC must use `B8G_ARENA_V1`, named pipes / Unix domain sockets (`\\.\pipe\b8g-host-bus` / `/run/b8g/host-bus.sock`), or CDP pipes — never local HTTP loopback servers.
4. **Zero WSL for Native Builds:** Cross-compile native C/C++/WASI targets directly via `holo-compiler` and Zig (`zig cc` / `zig c++`), never via WSL.
5. **Honest Real-vs-Virtual Labeling:** Never claim virtual pins, stubs, or mocked checks as real compiled binaries or full end-to-end passes. Materialization telemetry and PR verification checklists must reflect exact observed reality.
6. **Line Endings & Hygiene:** All text files must use LF (`\n`) line endings (enforced via `.gitattributes`) and clean SPDX/license hygiene.
