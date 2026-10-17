# Contributing to Talos Protocol

Thank you for your interest in contributing to the **Talos Protocol** ecosystem! We welcome contributions to our core protocols, services, smart contracts, SDKs, and developer tooling.

## Developer Certificate of Origin (DCO)

All repositories in the `talosprotocol` organization enforce the [Developer Certificate of Origin (DCO)](https://developercertificate.org/) version 1.1. By submitting a pull request, you certify that:

> You have the right to submit the contribution under the open source license (Apache 2.0) indicated in the repository.

### How to Sign Off Your Commits

Include a `Signed-off-by` trailer in each commit message:

```text
commit message title

Detailed description of what changed.

Signed-off-by: Full Name <email@example.com>
```

You can automate this with Git using the `-s` / `--signoff` flag:

```bash
git commit -s -m "feat(core): implement zero-knowledge ratchet state verification"
```

Configure your local Git identity before committing:

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

---

## Development Workflow

1. **Fork & Branch**:
   - Fork the repository you wish to contribute to.
   - Branch off `main`:
     ```bash
     git checkout -b feature/your-feature-name
     # or
     git checkout -b fix/issue-description
     ```

2. **Commit Convention**:
   We follow [Conventional Commits](https://www.conventionalcommits.org/):
   - `feat:` A new feature or capability
   - `fix:` A bug fix
   - `docs:` Documentation improvements
   - `security:` Security patch or hardening
   - `refactor:` Code restructuring without functional changes
   - `test:` Adding or modifying tests
   - `perf:` Performance optimizations
   - `chore:` Build tooling, workflow, or dependency updates

3. **Security & Secrets Guardrail**:
   - **NEVER** commit private keys, API tokens, mnemonics, passwords, or production credentials to any repository.
   - Use environment variables (via git-ignored `.env` files) for local testing.
   - Any commit exposing secrets will be rejected and blocked by our automated PR guardian bot.

4. **Testing & Quality Assurance**:
   - Run local linting and test suites before submitting your pull request.
   - Ensure all new features or bug fixes include corresponding unit, integration, or contract tests.

5. **Submitting a Pull Request**:
   - Push your branch to your fork.
   - Open a PR targeting `main`.
   - Provide a clear summary of changes in the PR description using our standard pull request template.
   - Ensure all CI checks and automated guardian bot reviews pass.

---

## Security Vulnerabilities

If you discover a security issue or vulnerability, **do not open a public GitHub issue**. Please report it securely via GitHub Private Vulnerability Reporting or email [security@talosprotocol.com](mailto:security@talosprotocol.com) as detailed in [SECURITY.md](SECURITY.md).

---

## Code of Conduct

Participation in the Talos Protocol community is subject to our [Code of Conduct](CODE_OF_CONDUCT.md). Please treat all members with respect and kindness.
