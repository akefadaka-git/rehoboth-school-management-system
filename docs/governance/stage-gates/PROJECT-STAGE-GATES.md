# R-SMS project stage gates

Owner-governed, sequential stages. Approval of one stage does not approve the next.

| Stage | Purpose | Status | Gate |
|---|---|---|---|
| A1 | Assessment, requirements, architecture, specifications and baseline | **OPEN / IN PROGRESS** | Explicit Owner approval/freeze |
| A2 | Read-only reconciliation of requirements, evidence, constraints and gaps | **NOT STARTED** | Starts only after A1 approval; closes with evidence-backed report |
| A3 | Implementation | **NOT AUTHORIZED** | A1 frozen + A2 completed/closed + separate Owner authorization |
| A4 | Verification and acceptance | **NOT STARTED** | Requires implementation scope and acceptance criteria |
| A5 | Deployment | **NOT STARTED; separate approval** | Requires A4 verification and explicit deployment authorization |

## Current authorization
Documentation reconstruction and organization only. No application code, migrations, production data import, deployment configuration, hosting commitment, paid service or expenditure is authorized. No merge or deployment without separate approval. A5 is a distinct gate.

Repository visibility remains Public until after deployment per OD-RSMS-006.

## Evidence and reporting
Record scope, authority, input provenance, deliverable/version, unresolved risks, approval date and exact approval statement, repository SHA/branch/PR, tests and verification evidence. Use statuses precisely: PASS, VERIFIED-CLOSED, PARTIAL, MISSING, UNRESOLVED, UNKNOWN, NOT RUN, NOT AUTHORIZED.

Current: A1 PARTIAL (reconstructed baseline; OD-RSMS-008 dispositioned the institutional-authority basis for the A1 project baseline; operational authority, finance/cash, academic, privacy and technical requirements remain open); A2 NOT STARTED; A3 NOT AUTHORIZED; A4/A5 NOT STARTED. No further church or academy documents are to be requested from the Owner.