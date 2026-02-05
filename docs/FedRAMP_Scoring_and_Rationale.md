# FedRAMP Moderate Scoring & Rationale

## Finding
Routing trust boundary bypass enables privileged administrative access to the Azure control plane outside the approved broker boundary.

## Pre-Mitigation Scoring
- Likelihood: Medium (2)
  - Routing trust failures are plausible in hybrid environments due to complexity and change frequency.
- Impact: High (3)
  - Azure administrative control plane exposure is high impact due to potential unauthorized configuration changes and audit assurance loss.

### Risk Score
2 × 3 = 6 → Medium

## Primary Control Family
- SC — System & Communications Protection (boundary enforcement / routing controls)

## Secondary Control Family
- AC — Access Control (privileged access governance expectations)

## Post-Mitigation (Residual) Scoring
- Residual Likelihood: Low (1)
  - Enforced routing/NSG controls + monitoring expectations reduce recurrence probability.
- Impact remains High (3)

### Residual Risk Score
1 × 3 = 3 → Low
