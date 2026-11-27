# R-SMS Stage Gates and Authorization Boundaries

## A1 — Assessment and specification
**Purpose:** Establish institutional facts, requirements, policy constraints, architecture proposals, risk register and acceptance criteria.

**Exit evidence:** Complete versioned A1 package, source/provenance register, unresolved-decision register and explicit Owner approval.

**Current status:** OPEN / IN PROGRESS.

## A2 — Read-only reconciliation
**Entry condition:** A1 explicitly approved.

**Purpose:** Reconcile the approved specification against authoritative institutional documents, existing systems (if any), operational workflows, data sources, hosting constraints and legal/privacy requirements.

**Boundary:** Read-only inspection and reporting. No application implementation, schema mutation, production data changes, deployment or merge.

**Exit evidence:** Reconciliation matrix, evidence references, gap disposition, risk assessment and explicit Owner closure.

## A3 — Implementation
**Entry condition:** A1 approved, A2 closed, and separate explicit A3 authorization.

**Purpose:** Implement only the approved scope using controlled branches, reviews, tests and traceable commits.

**Boundary:** No expansion into unapproved domains or production data. Preserve unrelated changes. No merge or deployment without separate authorization.

## A4 — Verification
**Entry condition:** A3 implementation scope is complete and submitted for verification.

**Purpose:** Verify functional behavior, security, privacy, accessibility, localization, data integrity, backup/recovery and operational readiness against approved acceptance criteria.

**Exit evidence:** Test results, defect disposition, security review, traceability matrix and explicit verification decision.

## A5 — Deployment
**Entry condition:** A4 verification accepted and separate deployment authorization provided.

**Purpose:** Controlled release, environment configuration, backup, rollback, operational handover and post-deployment checks.

**Boundary:** Deployment approval does not automatically authorize unrelated spending or scope changes.

## Repository visibility lifecycle
The repository remains Public during development by Owner decision. After deployment, change to Private only after a separate explicit Owner authorization and verify the resulting GitHub visibility. Do not schedule or automate the visibility change without that authorization.

## Status vocabulary
- **PASS:** Evidence demonstrates the criterion is satisfied.
- **VERIFIED-CLOSED:** Evidence reviewed and the item formally closed.
- **PARTIAL:** Some but not all required evidence or work is complete.
- **MISSING:** Required evidence or artifact has not been supplied or located.
- **UNRESOLVED:** Conflicting or incomplete information requires a decision.
- **UNKNOWN:** Not established.
- **NOT RUN:** Verification has not been executed.
- **NOT AUTHORIZED:** Work is outside the current approved scope.