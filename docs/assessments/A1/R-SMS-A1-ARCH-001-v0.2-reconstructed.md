# R-SMS-A1-ARCH-001 — A1 Assessment and Architecture Baseline

**Version:** 0.2 — reconstructed from available chat history; updated with Owner decisions  
**Date:** 27 November 2026  
**Institution:** Koybe Rehoboth Academy, Koybe, South Omo, Ethiopia  
**Status:** A1 OPEN / IN PROGRESS — NOT APPROVED OR FROZEN  
**Provenance:** This is a structured reconstruction, not a verbatim recovery. See [RECONSTRUCTION-NOTE.md](RECONSTRUCTION-NOTE.md).

## 1. Executive summary
R-SMS is proposed as a full School Management ERP for Koybe Rehoboth Academy. It is intended to improve manual/paper-based school administration through an integrated, secure, Amharic-first, mobile-responsive platform. Planning enrollment range: approximately 100–300 students. Proposed direction: modular monolith with API-first boundaries. Technology stack remains TBD.

## 2. Project charter and scope
Initial institution: Koybe Rehoboth Academy. Scope: full school ERP. Proposed access: web and mobile-responsive. Language: Amharic-first with English. Initial currency: ETB. Ethiopian and Gregorian calendar support to be assessed. Architecture should allow future multi-school expansion. Offline-tolerant workflows should be assessed. No implementation, migrations, production import, hosting/deployment, expenditure or paid-service commitment is included in this A1 activity.

## 3. Institutional assessment
**OWNER DECISION (27 Nov 2026):** Koibe Kale Hiwot Church owns and operates the academy. Official registration, governing instruments, ownership records and delegated authority documents remain to be collected. Current operations are described as manual/paper-based. Map actual forms, registers, approval records and retention practices before automation. Enrollment range is a planning estimate, not a verified count. Organizational chart and authority matrix remain unresolved.

## 4. Academic assessment
**OWNER DECISION:** Academy offers Kindergarten and Grades 1–6.  
**OWNER DECISION:** Academic year has two semesters.  
Unresolved: KG naming, grade conventions, sections, class-size limits, subjects, semester dates, calendar rules, exam/reporting periods, grading scale, assessment weights, pass marks, promotion/repetition, transfer and withdrawal policies.

Proposed capabilities: admission/enrollment/re-enrollment; grade/section assignment; curriculum/subject setup; semester records; attendance and discipline; assessments/exams/marks/report cards; transfer and historical record retention. Promotion rules must be configurable; no automatic promotion without authorized approval and audit record.

## 5. Financial assessment
**OWNER DECISION:** School fees are currently collected in cash only. Initial workflow should support fee schedules, student billing, cash receipts, collection register, cashier accountability, daily cash reconciliation and auditable adjustments. This does not approve future digital payments.

**OWNER DECISION:** Budget and major expenses use a shared approval policy. Roles, thresholds, categories, request/review/approval/payment workflow, escalation, emergency exceptions and segregation-of-duties rules remain unresolved.

Proposed capabilities: billing, fee schedules, scholarships/waivers, cash receipts, cashier sessions/cash custody, daily reconciliation, expense requests/approvals, budgets, accounting and payroll capability subject to confirmed requirements. Controls: unique receipt numbers, cashier identity, transaction references, duplicate detection, reversal/refund controls and audit history. Never silently edit/delete financial transactions; use controlled reversals/adjustments.

Historical planning figures in earlier context (unverified; not current operating expenses, approved budget, payroll, tuition or balances):
| Category | ETB |
|---|---:|
| Teacher salaries/support | 517,690 |
| Books | 343,200 |
| Educational materials | 150,000 |
| **Total** | **1,010,890** |

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

## 7. Proposed technical architecture
Modular monolith with API-first boundaries is the proposed initial style, subject to approval. Final language, framework, database, hosting, deployment and mobile/PWA choices remain TBD. Assess local maintainability, available skills, affordability, security lifecycle, backup/recovery, Amharic/Ethiopian calendar support, intermittent connectivity, portability and future scale. Avoid microservices unless evidence justifies the operational overhead.

Logical layers: responsive presentation; application/API (auth, authorization, validation, workflow); domain modules; relational persistence and controlled document storage; integrations only when approved. Offline queue/cache/sync and conflict handling require assessment; offline mode must not bypass authorization, audit or financial controls.

## 8. Data architecture
Use stable internal student identifiers; preserve historical enrollment, class assignments, attendance and results; distinguish people, student records, guardians, staff and organizational units; enforce referential integrity and controlled status transitions; retain audit history; define document classification, retention, backup and access rules; minimize personal data. A2 should inventory actual paper forms/registers. Do not publish real student or staff data in this public repository.

## 9. Identity, access and security
Proposed RBAC scoped by role, institution, class, student/guardian relationship and responsibility. Technical administration does not confer financial approval authority. Assess secure authentication/session management, least privilege, encryption in transit and at rest as appropriate, restricted child-data access, audit logs, secrets management, backup/restore testing, vulnerability/dependency management, incident response and access revocation. These are requirements to assess, not implemented controls.

## 10. Localization and accessibility
Amharic-first with English support; Ethiopian and Gregorian calendar support; ETB initial base currency; local date/number/text formatting; responsive mobile layouts; assess WCAG 2.2 AA. Test Amharic fonts, input, search, sorting and report rendering.

## 11. Proposed roles
Potential categories: Owner/governing authority, school leadership, academic leadership, teachers, registrar, finance officer, cashier, HR, librarian, procurement/storekeeper, parent/guardian, age-appropriate student, system administrator and auditor. This is not an approved authority matrix; exact roles and permissions remain unresolved.

## 12. Privacy, legal and compliance
No legal compliance determination has been made. Identify applicable Ethiopian education, child protection, privacy/data protection, employment, finance, tax, records and electronic transaction requirements; obtain qualified review. Collect institutional registration, school approvals/licenses, policies, forms and regulator guidance. Do not claim compliance until requirements are mapped and verified.

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
Expected A1 outputs: project charter/scope; institutional and operational assessment; stakeholder/responsibility map; functional and non-functional requirements; domain catalogue; data model; technical/technology assessment; security/privacy architecture; localization/accessibility requirements; integration/offline strategy; roadmap/acceptance criteria; unresolved decision/evidence register. Not all are complete in this reconstructed baseline.

## 15. Unresolved decisions and evidence
**Critical:** official registration/ownership; governing body and delegated authority; expense approval roles/thresholds/escalation; tuition/registration fee schedules; cashier/cash custody/receipt numbering/daily reconciliation; expense categories/budget procedure; payroll/accounting; privacy/retention/legal review.

**Academic/operational:** KG levels; sections/class sizes; year and semester dates; Ethiopian calendar rules; subjects; grading/assessment weights/pass marks; promotion/repetition/transfer; attendance/discipline; parent access; staff structure.

**Technical:** devices, connectivity, power; hosting and operating costs; backup/recovery objectives; offline priorities/conflict policy; document retention/export; integrations; users/concurrency/growth.

## 16. A1 acceptance criteria
Submit A1 for Owner approval only when scope/exclusions/stakeholders are documented; institutional, academic and financial workflows assessed; requirements uniquely identified and source-traceable; functional/non-functional requirements reviewed; domain and technical architecture documented; technology options and operating constraints evaluated; security/privacy/child-data/audit requirements specified; localization/accessibility specified; finance approval and cash-control gaps resolved or explicitly accepted as risks; assumptions, dependencies and risks visible; deliverables and acceptance criteria complete enough for an informed decision. Approval must be explicit, dated and version-specific.

## 17. Current disposition
A1 **OPEN / IN PROGRESS**; A2 **NOT STARTED**; A3 **NOT AUTHORIZED**; A4/A5 **NOT STARTED**. Implementation and deployment have not been authorized. This reconstruction is not itself an A1 approval.