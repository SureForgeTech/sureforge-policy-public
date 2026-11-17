# Continuous Monitoring Workflow

Policy Forge supports continuous monitoring by keeping findings, controls, evidence, and POA&M records connected.

When posture changes, reviewers can see whether the change came from a new finding, remediated issue, accepted risk, waiver, or assessment update.

## Accepted risk

Accepted risk is counted separately from open findings. Each acceptance records a reason and can carry an expiry date. When an acceptance expires, the finding returns to open on dashboards and finding lists.

## POA&M timeliness

POA&M timeliness shows `UNKNOWN`, not `PASS`, when serious findings have no POA&M. Missing records never read as compliant. The **Generate missing POA&Ms** action creates POA&M records for those findings so timeliness can be measured.
