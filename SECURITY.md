# Security Policy

Do not open public issues for vulnerabilities.

Report privately via **Security Advisories** on
[rl-lang/rl-lang](https://github.com/rl-lang/rl-lang/security/advisories/new).
Include the version, what you ran, and what you expected to be safe.

What counts: sandbox escapes in `rl run`, unsound `unsafe` in the
toolchain, supply-chain issues in releases and install scripts,
credential leaks in CI workflows.

Out of scope for this policy but still welcome as normal issues:
panics on bad input, wrong diagnostics, slow code paths.

We aim to acknowledge within a week and fix before disclosing. The
full policy lives at
[rl-lang/SECURITY.md](https://github.com/rl-lang/rl-lang/blob/main/SECURITY.md).
