# Rehoboth Academy School Management System (R-SMS)

Owner-governed school management ERP for Rehoboth Academy, Koybe, South Omo, Ethiopia.

## Project status

- **Current stage:** A1 — assessment and specification
- **A1 status:** OPEN / IN PROGRESS
- **A2:** NOT STARTED
- **A3 implementation:** NOT AUTHORIZED
- **A4 verification:** NOT STARTED
- **A5 deployment:** NOT STARTED
- **Repository visibility:** Public during development; planned transition to Private only after deployment, subject to a separate Owner-authorized action.

This repository currently holds project documentation only. It does not authorize application implementation, production data processing, expenditure, deployment, or operational use.

## Confirmed Owner-provided decisions

Recorded on 27 November 2026:

1. Koibe Kale Hiwot Church owns and operates Rehoboth Academy.
2. Budget and major expenses are governed through a shared approval policy. Specific roles, thresholds, workflow stages, and escalation rules remain unresolved.
3. The academy serves Kindergarten and Grades 1–6.
4. The academic year is organized into two semesters.
5. School fees are currently collected in cash only.

These are Owner-provided statements, not independently verified legal or institutional findings. See [Owner decisions](docs/governance/owner-decisions/2026-11-27-owner-decisions.md).

## Initial project context

- Location: Koybe, South Omo, Ethiopia.
- Intended scope: full School Management ERP.
- Approximate enrollment planning range: 100–300 students; to be validated.
- Current operating model: manual / paper-based; to be assessed.
- Initial platform direction: web-based and mobile-responsive.
- Languages: Amharic-first with English support.
- Calendar support: Ethiopian and Gregorian calendars.
- Initial currency: ETB.
- Architecture direction: modular monolith with API-first boundaries; proposal pending A1 approval.
- Offline-tolerant workflows and hosting approach require assessment.

## Documentation map

- `docs/governance/` — Owner decisions, authority, approval policy and stage gates.
- `docs/requirements/` — Institutional, academic and financial requirements.
- `docs/architecture/` — Proposed domains, data, security and localization architecture.
- `docs/assessments/A1/` — A1 assessment and specification records.
- `docs/decisions/ADRs/` — Architecture decision records.
- `docs/roadmap/` — Stage-gated delivery roadmap.

## Governance rules

- Distinguish confirmed facts, Owner decisions, proposals, assumptions, and unresolved matters.
- Give each Owner decision a unique ID, date, provenance, status, and affected artifacts.
- Preserve historical versions. Amendments must supersede and link to prior records rather than silently overwrite them.
- A stage is not approved or closed without explicit Owner approval and evidence.
- A2 is read-only reconciliation. A3 requires A1 approval and A2 closure.
- A4 verification and A5 deployment require their own evidence and approvals.
- Do not publish student, parent, staff, financial-account, credential, or other sensitive operational data in this public repository.

## Important notice

This repository is public during development by Owner direction. Public visibility is not permission to publish confidential institutional information or personal data. The planned post-deployment visibility change must be separately authorized and verified; it must not happen automatically.

## Current next step

Complete A1 assessment, resolve critical institutional and financial authority gaps, and present the full A1 baseline for explicit Owner review and approval.
