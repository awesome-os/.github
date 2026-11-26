## Summary

<!-- Describe what this PR changes and why. -->

## Tracking & Commit Trailers

<!-- Ensure your commits and/or PR description include the canonical trailers below. -->

- `Bug: awesome-os/awesome-os#<id>`
- `Materializes: <pkg>@<ver>` *(if applicable)*
- `Verified-By: holo-ci@v1` *(if applicable)*

## Verification Checklist

- [ ] `holo-ci verify` passes with zero violations
- [ ] `Holo-E2E` / relevant unit and integration test suites pass after the final edit
- [ ] SPDX headers and LF (`\n`) line endings verified across all modified text files
- [ ] Workspace invariants respected (hermetic `bin/` shims, `pnx` instead of `npx`, zero local HTTP IPC `B8G016`, zero WSL for native builds)
- [ ] Zero virtual-as-real claims (all reported binaries, CAS digests, and test scopes reflect exact observed results)
