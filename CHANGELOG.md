# Changelog

This file is the operator-facing release ledger. Every pull request adds one
line under `## Unreleased` with one of the allowed section labels, or
applies the `changelog-skip` label for a purely no-impact change. See EAS
§B2 Universal PR Essentials.

Allowed entry labels:

- `[BREAKING]` - incompatible API, data, deployment, or operator change.
- `[FEATURE]` - new user-visible or operator-visible capability.
- `[FIX]` - bug fix or compatibility repair.
- `[INTERNAL]` - tests, CI, docs, refactors, generated artifacts, or process.
- `[SECURITY]` - vulnerability fix, security control, or hardening change.

PR title prefix matches the highest-tier label added:
`[BREAKING]` -> `[major]`, `[FEATURE]` -> `[minor]`, others -> `[patch]`.

## Unreleased

### [BREAKING]

- None.

### [FEATURE]

- Document release v4.4.0 capabilities: reversible import removal with two-person approval, accepted risk counted separately with a reason and optional expiry, and POA&Ms for findings synced from integrations (README, continuous monitoring and ISSO workflows).
- Document POA&M timeliness showing `UNKNOWN` when serious findings have no POA&M, and the **Generate missing POA&Ms** action.
- Add v4.4.0 security principles to `docs/security/security-model.md` and release image signing, SBOMs and scan reports to `docs/security/sbom-and-supply-chain.md`.
- Note AWS Security Hub, Inspector and GuardDuty control mapping, and the current auto-close limitation, in the roadmap pages.

### [FIX]

- Point `SECURITY.md`, `docs/security/vulnerability-disclosure.md` and `NOTICE` at the moved and renamed repository `SureForgeTech/sureforge-policy-public`.
- State the supported container platforms and that Kubernetes deployment is no longer offered; drop Kubernetes from the image contract's secret-mount note.
- Document that the image contains no `curl` and give the health probe command; list the vulnerability scan reports among release verification files.
- Point `SECURITY.md` and `docs/security/vulnerability-disclosure.md` at the enabled GitHub private vulnerability reporting channel instead of an unnamed one.

### [INTERNAL]

- Wire scripts/check-no-private-paths.sh into the secret-scan workflow so CI validates private path and identifier restrictions on every pull request and push to main (#23).
- Pull requests are now welcome with a DCO sign-off (`git commit -s`): `CONTRIBUTING.md` says so, and a new `dco` workflow checks the sign-off on pull requests from outside contributors.
- State in `CONTRIBUTING.md` that issues are welcome and outside pull requests are not accepted for now, and label the pull request checklist as a maintainer step.
- `NOTICE` now names SureForgeTech as the copyright holder and in the attribution line; the CC BY 4.0 licence text is unchanged.
- Regenerate the fleet-core block in `AGENTS.md` to the current standard.
- Refresh the generated fleet core while preserving public repository guidance.
- Replace `CODE_OF_CONDUCT.md` with the Contributor Covenant 2.1, with a named enforcement contact.

- Route the four workflows to the org's self-hosted runners (`LINUX_RUNNER_LABELS`, `MACOS_RUNNER_LABELS`); install Node via `actions/setup-node` and lychee and gitleaks as checksum-verified, architecture-matched binaries in user space.
- Adopt the fleet agent-file standard: `AGENTS.md` with the shared core and repository rules (including the public-repository text guard), and a `CLAUDE.md` that only imports it.
- CI hygiene: every workflow job has a `timeout-minutes` sized from its recorded run times, and the three pull-request workflows cancel a superseded pull-request run (push-to-main runs are never cancelled).

### [SECURITY]

- None.
