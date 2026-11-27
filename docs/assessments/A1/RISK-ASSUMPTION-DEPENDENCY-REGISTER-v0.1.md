# A1 Preliminary Risk, Assumption and Dependency Register

**Artifact:** R-SMS-RAD-001  
**Version:** 0.1 — preliminary  
**Date:** 27 November 2026  
**Status:** PARTIAL — not approved or frozen

Likelihood and impact are qualitative preliminary assessments, not measured probabilities. Risk owners below are proposed accountable roles, not confirmed appointments. The register must be validated with the institution.

## Risks

| ID | Risk | Likelihood | Impact | Proposed owner | Mitigation / evidence needed | Status |
|---|---|---|---|---|---|---|
| RSK-001 | Legal ownership, school registration or operating authority differs from the current Owner-provided description or is not adequately documented. | Medium | Critical | Church governing authority | Obtain and reconcile registration, governing instruments, licenses and operating records before production setup. | OPEN |
| RSK-002 | Budget and major-expense approval roles or thresholds are unclear, allowing unauthorized commitments or payments. | High | Critical | Church governing authority | Approve written delegation matrix, monetary thresholds, segregation of duties, exceptions and audit requirements. | OPEN |
| RSK-003 | Cash collection lacks clear cashier custody, receipt sequence, reconciliation and reversal controls. | High | High | School leadership / finance authority | Document current cash process; define cashier assignment, receipt issuance, daily close, variance escalation and reversal approval. | OPEN |
| RSK-004 | Student/child personal information could be exposed through public repository content, weak access controls or unsafe exports. | Medium | Critical | School leadership / privacy responsible role | Keep real records and identifiers out of public Git; define data classification, access, retention, disclosure and incident controls. | OPEN |
| RSK-005 | Requirements inferred from incomplete chat history may not match actual school workflows or policies. | High | High | Project Owner / school stakeholders | Validate requirements against institutional documents, actual forms/registers and stakeholder walkthroughs during authorized A2. | OPEN |
| RSK-006 | Academic calendar, KG structure, grading and promotion rules are not yet specified. | High | High | Academic leadership | Obtain approved calendar, curriculum, grading, assessment and promotion policies. | OPEN |
| RSK-007 | Connectivity, power, device and local support constraints may make the selected architecture impractical. | Medium | High | School leadership / technical lead | Conduct site and user/device assessment; evaluate offline needs, hosting options and support capacity before technology selection. | OPEN |
| RSK-008 | Unverified historical financial estimates may be mistaken for current or approved figures if published. | Medium | High | Finance authority / Project Owner | Exclude such figures from the public baseline until source, date, meaning and disclosure authorization are verified. | MITIGATED IN PUBLIC BASELINE; source verification pending |
| RSK-009 | Backup, restore, incident response and vendor access arrangements may be inadequate for sensitive school records. | Medium | High | Technical lead / school leadership | Define data location, vendor access, RPO/RTO, backup encryption, restore testing and incident ownership before production. | OPEN |
| RSK-010 | Scope expansion across many ERP domains may exceed available budget, skills and operational capacity. | High | High | Project Owner / school leadership | Prioritize by validated need, stage delivery, estimate total cost and require approval for scope changes. | OPEN |

## Assumptions

| ID | Assumption | Validation required | Status |
|---|---|---|---|
| ASM-001 | Current school processes are predominantly manual/paper-based. | Observe and inventory actual registers, forms and work practices. | UNVERIFIED |
| ASM-002 | Planning enrollment range is approximately 100–300 students. | Confirm current student count and expected growth. | UNVERIFIED |
| ASM-003 | Web/mobile-responsive access is a suitable initial delivery model. | Validate devices, connectivity, user skills and accessibility needs. | PROPOSAL |
| ASM-004 | Amharic-first with English support is the desired interface direction. | Confirm terminology, translation review and reporting needs. | PROPOSAL |
| ASM-005 | ETB is the initial reporting currency. | Confirm accounting and reporting policy. | PROPOSAL |

## Dependencies

| ID | Dependency | Needed before | Status |
|---|---|---|---|
| DEP-001 | Institutional registration, licenses and governing instruments | A1 freeze / A2 reconciliation | MISSING |
| DEP-002 | Delegated authority and budget/expense approval policy | Finance workflow design and A1 freeze | MISSING |
| DEP-003 | Fee schedule and cash handling/reconciliation procedures | Finance requirements freeze | MISSING |
| DEP-004 | Academic calendar, curriculum, grading and promotion policies | Academic requirements freeze | MISSING |
| DEP-005 | Privacy, retention and applicable legal/regulatory review | A1 freeze / production design | MISSING |
| DEP-006 | Device, connectivity, power and support assessment | Technology selection | MISSING |
| DEP-007 | Approved technology/hosting options and operating-cost estimate | A1 architecture freeze | MISSING |

## Change and review controls

- Assign a named owner and due date to each risk and dependency during institutional review.
- Reassess likelihood, impact and residual exposure when evidence is obtained.
- Do not mark a risk closed solely because a proposed control is documented; require evidence that the control is approved and effective.
- Record risk acceptance by the authority empowered to accept it.
- This register is a preliminary planning aid and does not authorize A2, implementation, expenditure or deployment.
