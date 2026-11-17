# SBOM and Supply Chain

Policy Forge public materials encourage supply-chain hygiene:

- Maintain dependency visibility.
- Review third-party components.
- Use SBOMs where appropriate.
- Enable dependency alerts.
- Scan repositories for accidental credential exposure.

## Release images

Policy Forge release images ship with SBOMs and vulnerability scan reports, and are signed. Release files are listed in signed checksums, so a download can be verified before it is loaded. See the [container image contract](../deploy/image-contract.md#verification).

This repository does not include product dependency manifests.
