# NIST CSF 2.0 Maturity & Gap Assessment

**Project:** Amazon Supply Chain GRC Risk Register (independent, unofficial project — see README)
**Scope:** Assessment of the modeled organization's cybersecurity risk management maturity across all six NIST CSF 2.0 functions, based on the 58 risks documented in the accompanying risk register (`Amazon Supply Chain GRC Risk Register.xlsx`).

## Maturity Tiers (NIST CSF Implementation Tiers)

| Tier | Name | Description |
|---|---|---|
| 1 | Partial | Risk management practices are ad hoc, reactive, and not formalized. |
| 2 | Risk Informed | Practices are approved by management but not established as organization-wide policy. |
| 3 | Repeatable | Practices are formally documented, consistently applied, and regularly reviewed. |
| 4 | Adaptive | Practices are continuously improved based on lessons learned and predictive indicators. |

## Current State by Function

| Function | Current Tier | Target Tier | Key Gaps | Priority |
|---|---|---|---|---|
| Govern | 1 – Partial | 3 – Repeatable | No risk appetite statement; no C-SCRM policy; unclear third-party risk ownership; no executive oversight cadence | High |
| Identify | 2 – Risk Informed | 3 – Repeatable | Asset inventory coverage incomplete for OT/IoT warehouse devices | Medium |
| Protect | 2 – Risk Informed | 3 – Repeatable | Inconsistent access-control enforcement across vendor-managed systems | High |
| Detect | 2 – Risk Informed | 3 – Repeatable | Limited monitoring coverage of third-party system integrations | Medium |
| Respond | 2 – Risk Informed | 3 – Repeatable | No formal vendor-incident communication protocol | High |
| Recover | 3 – Repeatable | 3 – Repeatable | Recovery plans untested against vendor-outage scenarios | Low |

## Methodology

Each function's current tier was assessed by reviewing the risks documented against it in the risk register: the presence of open, high-severity Governance-related risks (no risk appetite statement, no policy review cadence, no executive oversight) placed **Govern** at Tier 1, since these are foundational governance practices that the rest of the framework depends on. Functions with documented but inconsistently enforced controls (e.g., **Protect**, **Detect**) were placed at Tier 2. **Recover** was assessed at Tier 3 based on documented recovery procedures, with the one open gap being validation against third-party/vendor-caused outages specifically.

## Remediation Roadmap

**Phase 1 (0–30 days) — Governance foundations**
- Draft and obtain executive/board sign-off on a formal risk appetite statement (addresses GV-001).
- Assign a single accountable owner (RACI) for third-party/vendor risk coordination (addresses GV-002, GV-008).

**Phase 2 (30–90 days) — Policy and oversight**
- Formalize a Cybersecurity Supply Chain Risk Management (C-SCRM) policy governing vendor onboarding, with a mandatory security review gate for OT/IoT vendors (addresses GV-003).
- Establish a quarterly executive risk-review cadence with mandatory escalation of overdue Critical/High risk items (addresses GV-005, GV-007).
- Establish an annual policy review cycle with designated policy owners (addresses GV-004).

**Phase 3 (90–180 days) — Operational hardening**
- Extend monitoring coverage to third-party/vendor system integrations (Detect).
- Test incident response and recovery plans specifically against vendor-outage and vendor-breach scenarios (Respond, Recover).
- Document organizational context and regulatory obligations, and link them explicitly to risk-scoring criteria (addresses GV-006).

## Outcome

Completing Phase 1–2 is projected to bring **Govern** from Tier 1 to Tier 2–3, closing the framework's largest gap and providing the accountability and policy foundation the other five functions depend on for sustained improvement.
