# R-SMS A1 — Assessment and Specification Status

**Document ID:** R-SMS-A1-ARCH-001  
**Known prepared version:** 0.2 — Updated with Owner decisions  
**Document date:** 27 November 2026  
**Stage status:** OPEN / IN PROGRESS  
**Approval status:** NOT FROZEN / NOT APPROVED

## Stage control

| Stage | Status | Boundary |
|---|---|---|
| A1 — Assessment, requirements and specification | OPEN / IN PROGRESS | Complete evidence review, requirements, architecture and unresolved decisions; submit for Owner approval. |
| A2 — Read-only reconciliation | NOT STARTED | Begins only after explicit A1 approval; no implementation or production changes. |
| A3 — Implementation | NOT AUTHORIZED | Requires A1 approval and A2 closure, plus explicit A3 authorization. |
| A4 — Verification | NOT STARTED | Requires implementation completion and a separately defined verification scope. |
| A5 — Deployment | NOT STARTED | Separate deployment approval required; post-deployment repository privacy transition is a separate Owner-authorized action. |

## A1 scope
Assess and specify a full School Management ERP for Rehoboth Academy, including institutional governance, students, academics, attendance, assessment, HR, finance, library, parent/guardian access, procurement/inventory, facilities/transport, communications, records, reporting, identity/security, configuration and integration.

This is a proposed module catalogue, not a frozen implementation commitment. Final scope and priorities require A1 review.

## Recorded Owner inputs
- Koibe Kale Hiwot Church owns and operates the academy.
- Budget and major expenses use shared authority under an approval policy; the detailed authority matrix is unresolved.
- Kindergarten and Grades 1–6 are offered.
- The academic year has two semesters.
- School fees are currently collected in cash only.
- The repository remains Public during development and changes to Private only after deployment, subject to separate authorization.

See [the Owner decision register](../../governance/owner-decisions/2026-11-27-owner-decisions.md).

## Proposed baseline directions — pending approval
- Web-based, mobile-responsive platform.
- Amharic-first user experience with English support.
- Ethiopian and Gregorian calendar support.
- ETB as initial base currency.
- Modular monolith with API-first boundaries.
- Future multi-school expansion considered in domain boundaries.
- Offline-tolerant workflows assessed for local connectivity conditions.
- Role-based access scoped by institutional responsibility, class, student relationship and assigned duties.
- Technical administration does not automatically confer financial approval authority.
- Financial records require traceable receipts, reconciliation, controlled reversal/refund, and audit history; no silent deletion or editing of posted transactions.

## Evidence and unresolved-decision register

| ID | Evidence / decision required | Priority | Status |
|---|---|---:|---|
| A1-GAP-001 | Official church/academy registration and ownership documentation | Critical | MISSING |
| A1-GAP-002 | Governing-body composition and delegated authority | Critical | UNRESOLVED |
| A1-GAP-003 | Budget and major-expense approval roles, thresholds and escalation | Critical | UNRESOLVED |
| A1-GAP-004 | Tuition, registration and other fee schedules | Critical | MISSING |
| A1-GAP-005 | Cashier assignment, cash custody, receipt numbering and daily reconciliation | Critical | UNRESOLVED |
| A1-GAP-006 | Expense categories, budget cycle and approval limits | Critical | UNRESOLVED |
| A1-GAP-007 | Payroll and accounting requirements | High | UNRESOLVED |
| A1-GAP-008 | Applicable privacy, child-data, retention and regulatory requirements | Critical | NOT ASSESSED |
| A1-GAP-009 | KG levels, grade naming, sections and class-size limits | Medium | UNRESOLVED |
| A1-GAP-010 | Academic year dates, semester dates and Ethiopian calendar rules | High | UNRESOLVED |
| A1-GAP-011 | Subject lists, grading scales, assessment weights and report-card rules | High | UNRESOLVED |
| A1-GAP-012 | Promotion, repetition, transfer and withdrawal policies | High | UNRESOLVED |
| A1-GAP-013 | Devices, connectivity, hosting, backup and recovery requirements | High | NOT ASSESSED |
| A1-GAP-014 | Parent/student access and communication policy | High | UNRESOLVED |
| A1-GAP-015 | Staff structure, roles and responsibilities | High | UNRESOLVED |

## A1 acceptance criteria
A1 may be submitted for approval only when:
1. Institutional ownership, governance and delegated authority are supported by available authoritative documents or explicitly listed as unresolved.
2. Functional and non-functional requirements are documented with provenance and priority.
3. Academic and financial workflows are specified, including exception paths and approval controls.
4. Data classification, privacy, security, access control, audit, backup and recovery requirements are documented.
5. Proposed domain architecture, integration boundaries, deployment assumptions and technology evaluation are documented.
6. Open questions, risks, assumptions, dependencies and exclusions are explicit.
7. A versioned A1 baseline and decision register are presented to the Owner for explicit approval.

## Evidence integrity notice
The A1 v0.2 document is referenced in the project record, but its complete original source file was not available during this repository setup. This file is a status/evidence register reconstructed from recorded project decisions and summaries; it is **not** a verbatim copy of A1 v0.2 and does not replace the original document.

The earlier v0.1 source was likewise not located. Preserve both original versions when their exact source artifacts become available; do not fabricate version history or claim an exact transfer.

## Authorization boundary
No application code, schema, migrations, tests, workflows, production data, deployment configuration or live service has been created or authorized by this document. A1 remains open.