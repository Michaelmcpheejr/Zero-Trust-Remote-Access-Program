# Sentinel Federal — Zero Trust Remote Access (GRC / FedRAMP Moderate Program)

This repository presents a consultant-style **GRC-led** Zero Trust Remote Access assessment for a GovFinTech organization (“Sentinel Federal”), aligned to **FedRAMP Moderate / NIST SP 800-53 (Moderate baseline intent)**.

## What this case study demonstrates
- Proper FedRAMP-aligned **scope definition** and assumptions
- A realistic Zero Trust failure mode: **routing trust boundary bypass**
- Risk articulation, asset/threat/vulnerability mapping
- Likelihood/impact scoring rationale and defensible risk rating
- Control-family anchoring (SC primary, AC secondary)
- Treatment decision (mitigate), remediation plan, and residual risk update
- Executive-ready briefing

## Scenario
- Organization: Sentinel Federal (GovFinTech), 20,000+ users, hybrid workforce
- Stack model: Azure, M365, Entra ID, hybrid AD, Intune, Splunk (conceptual), logical Zscaler broker
- Target: Azure administrative control plane
- Failure type: Network path bypass (routing trust boundary)

## Key documents
- Scope & Assumptions: docs/Scope_and_Assumptions.md
- Validation Method (No VM): docs/Validation_Method_NoVM.md
- Finding: docs/Routing_Trust_Bypass_Finding.md
- Risk Register: docs/Risk_Register.md
- FedRAMP Scoring Rationale: docs/FedRAMP_Scoring_and_Rationale.md
- Controls + Remediation Plan: docs/Controls_and_Remediation_Plan.md
- Residual Risk + Acceptance: docs/Residual_Risk_and_Acceptance.md
- Executive Briefing: docs/Executive_Briefing.md

## Evidence handling
Evidence is configuration and change-log based (NSG/UDR + Azure Activity Logs) due to workload constraints.
No production identifiers are included; screenshots are redacted.

## Role / Ownership
- McPhee — GRC lead: scope, risk articulation, scoring, control mapping, treatment, residual risk, executive brief
- Rayvaugn — networking support: diagrams and evidence capture (separate technical repo)
https://github.com/Rayvaugn1/Zero-Trust-Remote-Access-Program/tree/main
