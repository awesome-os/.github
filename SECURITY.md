# Security Policy

## Reporting a Vulnerability

The Awesome-OS organization takes security seriously across our operating system, runtime, browser, DevTools, AI platform, and Holo `v11` CAS infrastructure.

**Do NOT open public GitHub issues, pull requests, or discussions for suspected security vulnerabilities.**

Please report vulnerabilities privately through **GitHub Private Security Advisories**:

- **Primary (Private Advisory):** [https://github.com/awesome-os/awesome-os/security/advisories/new](https://github.com/awesome-os/awesome-os/security/advisories/new)
- **Email Fallback:** `security@awesome-os.com`

When submitting a report, please include:
- Target repository and affected component (e.g., `awesome-os`, `chromium-baseline`, `holo-v11`, `sectium-cloud-control-plane`, `sectium-device`).
- Affected commit SHA, release tag, or `v11` CAS SHA-512 artifact digest.
- Clear reproduction steps, proof-of-concept, or crash/sanitizer trace.
- Potential security impact and suggested mitigation, if known.

## Supported Versions

Security fixes are actively maintained for:

| Version / Channel | Supported | Notes |
| :--- | :---: | :--- |
| `main` branch across all 16 active org repositories | Yes | Primary development and continuous `holo-ci@v1` verification |
| Latest `v11-*` releases (including `v11-max-5os-latest`, `v11-oci-latest`, `v11-chromium-baseline-latest`, `v11-devtools-launchers-latest`) | Yes | Backported fixes and re-materialized CAS artifacts |
| Archived repositories (`129` read-only consolidated repos) | No | Preserved read-only for release provenance; report against the canonical target monorepo |

## Response SLA & Coordinated Disclosure

- **Acknowledgment SLA:** We acknowledge receipt of every valid security report within **48 hours**.
- **Triage & Assessment:** Initial severity triage and reproduction confirmation are typically completed within 5 business days.
- **Coordinated Disclosure:** We follow coordinated vulnerability disclosure. Please allow maintainers reasonable time to develop, verify, and publish patched `v11` CAS artifacts and advisories before public disclosure. Credit will be attributed in the published advisory upon request.
