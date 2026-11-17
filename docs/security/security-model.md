# Security Model

Policy Forge follows a public-safe security model centered on traceability, least privilege, evidence integrity, and human review.

## Principles

- Preserve source records.
- Keep remediation and attestation distinct.
- Require traceable rationale for compliance status changes.
- Treat AI output as advisory.
- Avoid hidden dashboard calculations.
- Support restricted and regulated operating models.
- Keep customer data inside its system boundary.
- Require two-person approval to remove imported data.
- Link OpenID Connect sign-in to existing accounts only by an email the identity provider marks as verified.
- Protect enrolled MFA from replacement.
- Refuse outbound integration and AI calls to cloud metadata addresses always, and to internal network addresses unless an operator allows a specific host.
- Keep client IP addresses and user IDs out of public metrics.
- Give new users a one-time invite link that expires after 7 days, so they set their own password.

This document intentionally avoids proprietary implementation detail, internal guardrail logic, deployment internals, and exploitable security information.
