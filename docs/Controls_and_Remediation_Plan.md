# Controls & Remediation Plan

## Treatment Decision
Mitigate

## Primary Controls (SC)
- Enforce approved routing and UDR governance
- Segment administrative control plane networks
- Explicitly deny non-brokered access paths

## Secondary Controls (AC)
- Require brokered pathways for privileged access
- Enforce least privilege and privileged role governance
- Monitoring expectations for access anomalies

## Monitoring
- Alert on privileged access events not originating from broker boundary
- Monitor routing and NSG changes affecting admin access
