# Contributing

## How to Contribute

Issues are welcome: bug reports, questions and ideas about the public Policy
Forge documentation. Pull requests from outside contributors are not accepted
for now, so that the project keeps a single copyright holder; a pull request
from outside may be closed without review. Open an issue describing the change
instead.

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
