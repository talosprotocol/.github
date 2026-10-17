# Talos Protocol Security Policy

The Talos Protocol project adheres to strict security standards across all cryptographic primitives, decentralized services, smart contracts, developer SDKs, and Model Context Protocol (MCP) bridges.

## Reporting a Vulnerability

**Please do NOT report security vulnerabilities through public GitHub issues, public PRs, or public community chat channels.**

We support and strongly recommend using **GitHub Private Vulnerability Reporting** directly within any repository in the [talosprotocol](https://github.com/talosprotocol) organization:
- Navigate to the **Security** tab of the relevant repository.
- Click **Report a vulnerability** to open an encrypted advisory draft visible only to project maintainers.

Alternatively, you can email our dedicated security response team:
- **Email**: [security@talosprotocol.com](mailto:security@talosprotocol.com)
- **PGP Key**: Available upon request or via standard keyservers.

### What to Include in Your Report

To help us triage and resolve your report as quickly as possible, please include:
1. **Affected Component**: Specific repository (e.g., `talos`, `talos-core-rs`, `talos-gateway`, `talos-contracts`), file path, and commit SHA/version.
2. **Vulnerability Type**: e.g., Cryptographic flaw, remote code execution, authentication bypass, replay attack, denial of service, secret exposure.
3. **Step-by-Step Reproduction**: Detailed steps, command invocations, network captures, or test scripts.
4. **Proof of Concept (PoC)**: Minimal working exploit or demonstration script if available.
5. **Impact Assessment**: What an adversary could achieve by exploiting this flaw.
6. **Suggested Remediation**: If you have identified a fix or mitigation.

### Response Timelines (SLA)

| Stage | Expected Timeline | Description |
|---|---|---|
| **Initial Acknowledgment** | Within 48 hours | Confirmation of report receipt and assignment to a security engineer. |
| **Triage & Assessment** | Within 7 days | Validation of vulnerability severity, scope, and affected versions. |
| **Fix Development** | 14 to 30 days | Private development, testing, and peer review of patches. |
| **Coordinated Disclosure** | Post-patch release | Public advisory publication and CVE assignment if applicable. |

### Supported Versions

Security updates and patches are actively maintained for the following branches:

| Project / Component | Active / Supported Version | End of Life / Unsupported |
|---|---|---|
| `talosprotocol/talos` | `main` | Older untagged snapshots |
| `talos-core-rs` | `main` (v0.1+) | Legacy prototypes |
| `talos-gateway` & `talos-ai-gateway` | `main` | Unsupported |
| `talos-contracts` | `main` (EVM/Solidity verified) | Deprecated drafts |
| Talos SDKs (`go`, `rust`, `ts`, `py`, `java`) | `main` (Latest minor release) | Pre-alpha versions |

### Safe Harbor

We consider security research conducted in good faith under this policy to be authorized. We commit to:
- Not pursuing legal action against researchers who discover and report vulnerabilities in accordance with this policy.
- Collaborating transparently with researchers to understand, validate, and remediate reported findings.
- Publicly crediting researchers in release notes and security advisories (unless anonymity is requested).
