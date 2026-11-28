# R-SMS-A1-ARCH-001 — A1 Assessment and Architecture Baseline

**Version:** 0.2 — reconstructed from available chat history; updated with Owner decisions  
**Date:** 27 November 2026  
**Institution:** Koybe Rehoboth Academy, Koybe, South Omo, Ethiopia  
**Status:** A1 OPEN / IN PROGRESS — NOT APPROVED OR FROZEN  
**Provenance:** This is a structured reconstruction, not a verbatim recovery. See [RECONSTRUCTION-NOTE.md](RECONSTRUCTION-NOTE.md).  
**Requirements companion:** [A1 Preliminary Requirements Register v0.1](../../requirements/A1-REQUIREMENTS-REGISTER-v0.1.md).

## 1. Executive summary
R-SMS is proposed as a full School Management ERP for Koybe Rehoboth Academy. It is intended to improve manual/paper-based school administration through an integrated, secure, Amharic-first, mobile-responsive platform. Planning enrollment range: approximately 100–300 students; this is an unverified planning estimate, not a measured count. Proposed direction: modular monolith with API-first boundaries. Technology stack remains TBD.

## 2. Project charter and scope
Initial institution: Koybe Rehoboth Academy. Scope: full school ERP. Proposed access: web and mobile-responsive. Language: Amharic-first with English. Initial currency: ETB. Ethiopian and Gregorian calendar support to be assessed. Architecture should allow future multi-school expansion, but the first deployment scope is the named academy unless separately approved. Offline-tolerant workflows should be assessed.

Excluded from this A1 activity: application implementation, migrations, production data import, hosting/deployment, expenditure, paid-service commitment and operational use. The public repository must contain documentation only and must not contain real student, parent, staff, credential, account or confidential operational data.

## 3. Institutional assessment
**OWNER DECISIONS (27–28 Nov 2026):** Koibe Kale Heywot Church owns and operates the academy. The Owner confirms that Ethiopian Kale Heywot Church registration is sufficient as the institutional-authority basis for this A1 project baseline; no further church or academy registration, constitution, bylaws or governance documents are to be requested from the Owner. This is an Owner-approved project basis, not a claim that a registration certificate was independently inspected or that all school-specific statutory permissions have been verified. Do not infer specific officeholder powers or approval thresholds. Current operations are described as manual/paper-based. Map actual forms, registers, approval records and retention practices before automation. Enrollment range is a planning estimate, not a verified count. Operational role assignments and authority matrix remain unresolved.

The system must distinguish institutional ownership, school operation, governance, delegated approval authority and technical administration. The institutional-authority basis for this A1 project baseline is the explicit Owner decision recorded as OD-RSMS-008. This does not establish unprovided individual officeholder powers, internal delegation limits or school-specific statutory permissions. Candidate stakeholders and responsibilities are listed in the requirements register; they are not an approved organization chart.

## 4. Academic assessment
**OWNER DECISION:** Academy offers Kindergarten and Grades 1–6.  
**OWNER DECISION:** Academic year has two semesters.  
Unresolved: KG naming, grade conventions, sections, class-size limits, subjects, semester dates, calendar rules, exam/reporting periods, grading scale, assessment weights, pass marks, promotion/repetition, transfer and withdrawal policies.

Proposed capabilities: admission/enrollment/re-enrollment; grade/section assignment; curriculum/subject setup; semester records; attendance and discipline; assessments/exams/marks/report cards; transfer and historical record retention. Promotion rules must be configurable; no automatic promotion without authorized approval and audit record. Detailed candidate requirements and acceptance criteria are in the companion requirements register.

## 5. Financial assessment
**OWNER DECISION:** School fees are currently collected in cash only. Initial workflow should support fee schedules, student billing, cash receipts, collection register, cashier accountability, daily cash reconciliation and auditable adjustments. This does not approve future digital payments.

**OWNER DECISION:** Budget and major expenses use a shared approval policy. Roles, thresholds, categories, request/review/approval/payment workflow, escalation, emergency exceptions and segregation-of-duties rules remain unresolved. Do not infer approval authority from job titles or technical permissions.

Proposed capabilities: billing, fee schedules, scholarships/waivers, cash receipts, cashier sessions/cash custody, daily reconciliation, expense requests/approvals, budgets, accounting and payroll capability subject to confirmed requirements. Controls: unique receipt numbers, cashier identity, transaction references, duplicate detection, reversal/refund controls and audit history. Never silently edit/delete financial transactions; use controlled reversals/adjustments.

Historical budget/planning figures mentioned in earlier project context are intentionally excluded from this public reconstruction. Their source, date, meaning, accuracy and authorization for public disclosure have not been independently established. They must not be treated as current expenses, approved budget, payroll, tuition or account balances. If needed, reconcile them through an appropriately restricted evidence process rather than publishing them here.

## 6. Proposed ERP domain catalogue
Proposal, not frozen requirements:
1. Governance and Administration
2. Student Management
3. Academic Management
4. Attendance and Discipline
5. Assessment and Examinations
6. Human Resources
7. Finance and Accounting
8. Library
9. Parent and Guardian Portal
10. Procurement and Inventory
11. Transport and Facilities
12. Communication
13. Documents and Records
14. Analytics and Reporting
15. Identity and Security
16. Configuration and Integration

Each domain requires scope boundaries, actors, records, workflows, interfaces and acceptance criteria. The catalogue is not an approved implementation decomposition.

## 7. Proposed technical architecture
Modular monolith with API-first boundaries is the proposed initial style, subject to approval. Final language, framework, database, hosting, deployment and mobile/PWA choices remain TBD. A documented options assessment must compare local skills and maintainability, lifecycle/security support, affordability and total operating cost, hosting constraints, backup/recovery, Amharic/Ethiopian calendar support, intermittent connectivity, portability and future scale. Avoid microservices unless evidence justifies the operational overhead.

Logical layers proposed for evaluation:
- Presentation: responsive web interface, localization and accessible interaction.
- Application/API: authentication, authorization, validation, workflow orchestration and reporting endpoints.
- Domain: bounded school capabilities with explicit ownership of business rules.
- Persistence: relational data with integrity constraints, migrations and controlled document storage.
- Operations: logs, audit, backup, restore, monitoring and support procedures.
- Integration: external interfaces only after need, authority, security and cost are assessed.

Offline queue/cache/sync and conflict handling require a use-case assessment. Offline mode must not bypass authorization, audit or financial controls. No deployment topology or technology has been selected.

## 8. Data architecture
Use stable internal student identifiers; preserve historical enrollment, class assignments, attendance and results; distinguish people, student records, guardians, staff and organizational units; enforce referential integrity and controlled status transitions; retain audit history; define document classification, retention, backup and access rules; minimize personal data. A2 should inventory actual paper forms/registers and reconcile required data fields, sources, custodians, access and retention.

A conceptual entity inventory should include institution/organizational unit, person, student, guardian relationship, staff, academic year, semester, grade, section, subject, enrollment, attendance, assessment, result, fee item, student charge, cash receipt, cashier session, expense request, approval, budget, document and audit event. This is a discovery inventory, not a frozen schema. Cardinalities, identifiers, history strategy, data quality, retention and reporting definitions remain to be designed and validated.

## 9. Identity, access and security
Proposed RBAC scoped by role, institution, class, student/guardian relationship and responsibility. Technical administration does not confer financial approval authority. Assess secure authentication/session management, least privilege, encryption in transit and at rest as appropriate, restricted child-data access, audit logs, secrets management, backup/restore testing, vulnerability/dependency management, incident response and access revocation. These are requirements to assess, not implemented controls.

A threat/risk assessment must cover account compromise, privilege escalation, insider misuse, child-data exposure, financial fraud, receipt manipulation, unauthorized exports, lost devices, insecure backups and service interruption. Specify threat actors, trust boundaries, preventive/detective controls, residual risk and test evidence before A1 approval.

## 10. Localization and accessibility
Amharic-first with English support; Ethiopian and Gregorian calendar support; ETB initial base currency; local date/number/text formatting; responsive mobile layouts; assess WCAG 2.2 AA as a proposed target. Test Amharic fonts, input, search, sorting and report rendering. Calendar conversion, date authority, language review and accessibility target require Owner/stakeholder confirmation.

## 11. Proposed roles
Potential categories: Owner/governing authority, school leadership, academic leadership, teachers, registrar, finance officer, cashier, HR, librarian, procurement/storekeeper, parent/guardian, age-appropriate student, system administrator and auditor. This is not an approved authority matrix; exact roles, permissions, separation of duties and delegations remain unresolved.

## 12. Privacy, legal and compliance
No legal compliance determination has been made. A public-source scan has identified the following material statutory requirements for the A1 design baseline:

- **General Education Proclamation No. 1368/2025:** Article 21 includes schools owned by religious institutions among general-education institutions; Article 75(1) states that non-governmental general-education institutions, including religious-institution-owned schools, must be registered by meeting school criteria; Article 80(1) assigns regional education offices authority to register, license and recognize such schools, and Article 80(2) requires license renewal every two years. Accordingly, OD-RSMS-008 remains the accepted Church institutional-authority basis for this project, but Church registration must not be treated as proof of Rehoboth Academy's separate school-level registration/licensing/accreditation status. That school-specific status is **UNKNOWN / NOT VERIFIED**; no further documents are requested from the Owner.
- **Licensing and Renewal of Schools in the General Education Sector, Directive No. 992/2016**, is listed by the Ministry of Justice with subsequent amendment Directive No. 1037/2025. The amendment published by the Ministry of Justice defines tuition-fee increases; the detailed current licensing criteria and applicability must be assessed from the full directive set before any compliance claim.
- **Personal Data Protection Proclamation No. 1321/2024:** Article 6 sets data-processing principles including specified lawful purposes, data minimization, accuracy, retention limitation, integrity/confidentiality/security and data sovereignty; Article 7 addresses lawful bases; Article 11 requires processing of minors' personal data to protect their rights and best interests, with parent/guardian/tutor authorization or vital-interest basis, reasonable age/authorization verification, and prohibits processing minors' data for marketing or profiling.

Official public sources:
- [General Education Proclamation No. 1368/2025 — Ministry of Justice](https://justice.gov.et/en/law/general-education-proclamation-no-1368-2025/) and [official Federal Negarit Gazette PDF](https://justice.gov.et/wp-content/uploads/2025/04/1368.pdf).
- [Directive No. 992/2016 — Ministry of Justice](https://justice.gov.et/en/directives/licensing-and-renewal-of-schools-in-the-general-education-sector-directive-no-992-2016/) and [Amendment No. 1037/2025](https://justice.gov.et/en/directives/general-education-sector-schools-licensing-and-renewal-directive-amendment-directive-no-1037-2025/).
- [Personal Data Protection Proclamation No. 1321/2024 — Ministry of Justice](https://justice.gov.et/en/law/personal-data-protection-proclamation/).

These are preliminary statutory-source findings, not legal advice or a determination of the Academy's current licensing status. Use publicly available authoritative Ethiopian legal/regulatory sources and qualified review to identify any further applicable school-specific obligations; do not request additional institutional documents from the Owner. Record any requirement that cannot be verified as an explicit limitation. Do not claim compliance until applicable requirements are mapped and verified.

Define data classification, lawful purpose/authority, minimum collection, guardian access, disclosure, correction, retention, archival, deletion, incident response, vendor access and cross-border processing questions. These require qualified legal and institutional review; this document is not legal advice or a compliance certification.

## 13. Staged roadmap
| Stage | Deliverable | Status |
|---|---|---|
| A1 | Assessment, requirements, architecture and baseline | OPEN / IN PROGRESS |
| A2 | Read-only evidence/requirements reconciliation and gap closure | NOT STARTED |
| A3 | Authorized implementation | NOT AUTHORIZED |
| A4 | Verification, security review, user acceptance and readiness | NOT STARTED |
| A5 | Deployment and handover; separate authorization | NOT STARTED |

A3 requires explicit A1 approval/freeze, A2 completion/closure and separate Owner authorization. A5 is separately gated.

## 14. Deliverable register
| A1 deliverable | Current state | Evidence / next action |
|---|---|---|
| Project charter and scope | PARTIAL | Reconstructed here; Owner review required |
| Institutional assessment and authority map | PARTIAL | Owner-approved institutional basis recorded; individual role/delegation details remain unresolved and must not be inferred |
| Academic and student workflows | PARTIAL | Validate calendars, grade structure, curriculum and policies |
| Finance and cash workflows | PARTIAL | Obtain fee schedule, cashier/cash custody and approval policy |
| Traceable requirements catalogue | PARTIAL | See companion register; validate with stakeholders |
| Domain catalogue | PARTIAL | Proposed domains listed; boundaries and ownership TBD |
| Data model | PARTIAL | Conceptual entity inventory only; relationships and retention TBD |
| Technology options assessment | MISSING | Compare feasible stack/hosting options and operating cost |
| Security/privacy threat assessment | PARTIAL | Initial control themes listed; formal threat and privacy review missing |
| Localization/accessibility requirements | PARTIAL | Targets and test cases need confirmation |
| Offline/integration strategy | MISSING | Assess use cases, connectivity and external dependencies |
| Risk/assumption/dependency register | PARTIAL | Critical gaps listed; likelihood, impact, mitigation and owners to be completed |
| Acceptance criteria and roadmap | PARTIAL | Stage gates recorded; measurable A1 exit evidence still required |

## 15. Unresolved decisions and evidence
**Critical:** school-specific registration/licensing/accreditation status under Proclamation 1368/2025 (unknown; separate from Church institutional authority); operational role assignments and delegated authority; expense approval roles/thresholds/escalation; tuition/registration fee schedules; cashier/cash custody/receipt numbering/daily reconciliation; expense categories/budget procedure; payroll/accounting; privacy/retention/legal review. The institutional-authority basis is Owner-dispositioned under OD-RSMS-008; do not reopen it by requesting more documents.

**Academic/operational:** KG levels; sections/class sizes; year and semester dates; Ethiopian calendar rules; subjects; grading/assessment weights/pass marks; promotion/repetition/transfer; attendance/discipline; parent access; staff structure.

**Technical:** devices, connectivity, power; hosting and operating costs; backup/recovery objectives; offline priorities/conflict policy; document retention/export; integrations; users/concurrency/growth; support and training model.

Each critical gap needs a responsible role, evidence source where applicable, due point, impact and disposition. A2 must perform read-only reconciliation after A1 approval; it must not invent missing policy or alter operational systems. Do not make additional institutional-document requests to the Owner; unresolved internal operating rules must be recorded for Owner decision or explicitly deferred.

## 16. A1 acceptance criteria
Submit A1 for Owner approval only when:
- Scope, exclusions, stakeholders and operating assumptions are documented.
- Institutional, academic and financial workflows have been assessed with relevant stakeholders.
- Requirements have stable IDs, source/provenance, priority, acceptance criteria and traceability.
- Functional and non-functional requirements are reviewed and measurable where applicable.
- Domain boundaries, conceptual data architecture and technical options are documented.
- Technology and hosting options are evaluated against affordability, local skills, security lifecycle and operational constraints.
- Security, privacy, child-data, access-control and audit requirements have a documented threat/risk assessment.
- Localization, calendar and accessibility requirements have testable acceptance criteria.
- Finance approval, cash custody, receipt and reconciliation gaps are resolved or explicitly accepted as risks by the appropriate authority.
- Assumptions, dependencies, risks, evidence gaps and decisions are visible with owners and dispositions.
- Deliverables, exclusions, risks and acceptance criteria are complete enough for an informed, version-specific Owner decision.

## 17. Current disposition
A1 **OPEN / IN PROGRESS**; A2 **NOT STARTED**; A3 **NOT AUTHORIZED**; A4/A5 **NOT STARTED**. Implementation and deployment have not been authorized. This reconstruction and its companion requirements register are not A1 approval.
