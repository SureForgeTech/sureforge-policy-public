# Contributing

## How to Contribute

Issues and pull requests are both welcome. For anything larger than a small fix,
open or comment on an issue first so we agree on the approach.

Sign off every commit with `git commit -s`. This adds a `Signed-off-by:` line
certifying the [Developer Certificate of Origin](https://developercertificate.org/):
you wrote the change or have the right to submit it under the licence in this
repository's `LICENSE` file, and your contribution comes under that licence. A
check confirms the sign-off on pull requests from outside contributors. Every
pull request gets review and must pass the required checks before a maintainer
merges it.

CodeRabbit (free open-source plan) may comment on pull requests. Its reviews are advice only and never required. On repositories with fewer than 10 stars it does not run on its own; comment `@coderabbitai review` to trigger it.

- For how to write a good issue, see the
  [SureForgeTech contributing guide](https://github.com/SureForgeTech/.github/blob/main/CONTRIBUTING.md).
- Do not report security problems in a public issue; follow
  [SECURITY.md](SECURITY.md).

## Public-Safe Content Only

Issues and changes must not include:

- Proprietary application source code
- Internal guardrail implementation logic
- Credentials or tokens
- Customer names or customer data
- Private deployment details
- Internal tickets
- Live infrastructure identifiers
- Exploit-ready security detail

Use synthetic examples and placeholders only.

## For Maintainers: Before Opening a Pull Request

Run:

```bash
./scripts/validate-public-repo.sh
```

Confirm that the pull request describes the documentation or demo change and explains why it is safe for public release.
