# A1 Preliminary Requirements Register

**Artifact:** R-SMS-REQ-001  
**Version:** 0.1 — preliminary reconstruction  
**Date:** 27 November 2026  
**Status:** PARTIAL — for A1 review; not approved or frozen  
**Source basis:** Retrievable ChatGPT project history and Owner decisions recorded in OWNER-DECISIONS-2026-11-27.md. OD-RSMS-008 confirms Ethiopian Kale Heywot Church registration as sufficient for the A1 institutional-authority project basis; no claim is made that a certificate was independently inspected.

This register makes candidate requirements traceable. It is not a claim that the workflows, policies or acceptance criteria have been validated with school personnel. Requirements marked OWNER are based on explicit Owner statements; PROPOSAL items require review. Priority: Must = foundational control/capability for the intended system; Should = important but scope/sequence requires confirmation; TBD = cannot be prioritized until evidence is obtained.

## 1. Institutional and governance requirements

| ID | Requirement | Source / class | Priority | Acceptance / verification criterion | Status |
|---|---|---|---|---|---|
| GOV-001 | Represent Koibe Kale Heywot Church as the Owner/operator relationship for Rehoboth Academy on the Owner-approved A1 project basis. | OD-RSMS-001 / OWNER | Must | Institutional record can represent the Owner-approved owner/operator relationship separately from school operating units; do not infer individual officeholder powers. Track school-specific registration/licensing/accreditation separately under General Education Proclamation No. 1368/2025, Articles 75 and 80. | PARTIAL |
| GOV-002 | Maintain a configurable organization, governance and delegated-authority model. | A1 context / PROPOSAL | Must | Roles, authority limits and delegations are documented, approved and versioned; no authority is inferred from a job title. | UNRESOLVED |
| GOV-003 | Support shared approval policy for budgets and major expenses. | OD-RSMS-002 / OWNER | Must | Authorized roles, thresholds, workflow states, segregation rules and escalation are configured from an approved policy. | PARTIAL |
| GOV-004 | Preserve approval decisions and changes in an auditable history. | Governance/security proposal | Must | Each approval records actor, role, timestamp, decision, reference and prior state; unauthorized alteration is prevented. | PROPOSAL |

## 2. Student and academic requirements

| ID | Requirement | Source / class | Priority | Acceptance / verification criterion | Status |
|---|---|---|---|---|---|
| STD-001 | Support student admission, enrollment and re-enrollment. | Full ERP scope / PROPOSAL | Must | Authorized registrar can create and update a student lifecycle record with unique internal identifier and required-field validation. | PROPOSAL |
| STD-002 | Support Kindergarten and Grades 1–6. | OD-RSMS-003 / OWNER | Must | Grade structure can represent KG and Grades 1–6; exact KG naming and section structure remain configurable pending confirmation. | OWNER-RECORDED |
| STD-003 | Support an academic year organized into two semesters. | OD-RSMS-004 / OWNER | Must | Each academic year has two configured semester periods with start/end dates and controlled status transitions. | OWNER-RECORDED; dates TBD |
| STD-004 | Preserve historical enrollment, class placement, attendance and assessment records. | Data architecture / PROPOSAL | Must | A student's prior-year records remain retrievable after promotion, transfer, withdrawal or re-enrollment. | PROPOSAL |
| ACA-001 | Configure subjects, assessments, examinations, grading scales and report cards. | Full ERP scope / PROPOSAL | Must | Academic administrator can configure a reviewed grading scheme; generated reports show the correct semester, subject and assessment values. | PROPOSAL |
| ACA-002 | Do not promote students automatically without authorized approval. | Governance control / PROPOSAL | Must | Promotion requires an authorized decision and records approver, date and rationale; automated bulk action cannot bypass approval. | PROPOSAL |
| ACA-003 | Configure attendance and discipline records with role-restricted access. | Full ERP scope / PROPOSAL | Should | Authorized staff can record and correct attendance with audit trail; access is limited by assigned class and responsibility. | PROPOSAL |
| ACA-004 | Define academic calendar dates and Ethiopian/Gregorian date presentation. | Owner context / PROPOSAL | Must | Academic calendar supports the approved local calendar rules and unambiguous date display; conversion is tested against approved examples. | UNRESOLVED |

## 3. Finance requirements

| ID | Requirement | Source / class | Priority | Acceptance / verification criterion | Status |
|---|---|---|---|---|---|
| FIN-001 | Initial school-fee collection workflow must support cash only. | OD-RSMS-005 / OWNER | Must | Fee payment can be recorded as cash with receipt and cashier attribution; no unapproved digital payment channel is enabled. | OWNER-RECORDED |
| FIN-002 | Support configurable fee schedules, student charges and balances. | Full ERP scope / PROPOSAL | Must | Authorized finance role can configure fee items and apply approved charges; totals reconcile to student account ledger. | PROPOSAL |
| FIN-003 | Issue uniquely identifiable cash receipts and retain receipt history. | Cash-control proposal | Must | Each receipt has unique number, date/time, cashier, student/account, amount and transaction reference; duplicates are detected. | PROPOSAL |
| FIN-004 | Support cashier accountability and daily cash reconciliation. | Cash-control proposal | Must | Cashier session totals, receipt sequence, voids/reversals and counted cash reconcile; variances require documented explanation and review. | UNRESOLVED |
| FIN-005 | Prevent silent editing or deletion of posted financial transactions. | Financial-control proposal | Must | Posted transaction changes occur only through authorized reversal/adjustment records linked to the original; audit history remains available. | PROPOSAL |
| FIN-006 | Implement shared budget and major-expense approval workflow only after authority rules are documented. | OD-RSMS-002 / OWNER | Must | Request, review, approval, payment and exception roles/limits are approved and segregated before configuration; system blocks unauthorized approvals. | UNRESOLVED |
| FIN-007 | Support payroll and accounting only to the extent confirmed by institutional requirements. | A1 scope / PROPOSAL | TBD | Approved payroll/accounting scope, chart of accounts, periods and statutory requirements are documented before design freeze. | UNRESOLVED |
| FIN-008 | Do not enable bank or online fee collection without a separate Owner decision. | OD-RSMS-005 / OWNER | Must | No digital payment integration is configured or exposed until a new recorded approval and security review exist. | OWNER-RECORDED |

## 4. Identity, privacy and security requirements

| ID | Requirement | Source / class | Priority | Acceptance / verification criterion | Status |
|---|---|---|---|---|---|
| SEC-001 | Enforce role- and responsibility-based access, scoped to institution, class and student/guardian relationship where applicable. | Security proposal | Must | Access tests demonstrate users can access only authorized records and functions. | PROPOSAL |
| SEC-002 | Separate technical administration from financial approval authority. | Governance/security proposal | Must | System administrator privileges do not grant budget, expense or payment approval permissions by default. | PROPOSAL |
| SEC-003 | Protect child/student personal data and restrict disclosure. | Personal Data Protection Proclamation No. 1321/2024, Arts. 6, 7 and 11 | Must | Document lawful purpose and basis, data minimization, accuracy, retention limitation, integrity/confidentiality/security, data sovereignty, minors' best interests, parent/guardian/tutor authorization or vital-interest basis, reasonable age/authorization verification, and prohibition on marketing/profiling minors; test controls before production. | LEGAL REQUIREMENTS IDENTIFIED; DESIGN UNRESOLVED |
| SEC-004 | Record security-relevant and financial actions in tamper-evident audit history. | Security proposal | Must | Audit events identify actor, action, target, timestamp and outcome; privileged access and retention are controlled. | PROPOSAL |
| SEC-005 | Define authentication, session, credential recovery and access revocation controls. | Security proposal | Must | Security design specifies controls and tests for account lifecycle, session expiry, recovery and prompt revocation. | UNRESOLVED |
| SEC-006 | Define backup, restore, incident response and recovery objectives. | Operational resilience proposal | Must | Approved RPO/RTO, backup schedule, restore test evidence and incident ownership are documented before production. | UNRESOLVED |
| SEC-007 | Track school-level registration, licensing and accreditation separately from the Church's institutional registration. | General Education Proclamation No. 1368/2025, Arts. 21(1)(h), 75(1), 80(1)–(2) | Must | System governance/compliance records can record issuing regional education office, school license/recognition reference, issue/expiry dates, renewal due date and status; no current Academy license status is assumed. | LEGAL REQUIREMENT IDENTIFIED; ACADEMY STATUS UNKNOWN |

## 5. Platform, localization and operations requirements

| ID | Requirement | Source / class | Priority | Acceptance / verification criterion | Status |
|---|---|---|---|---|---|
| NFR-001 | Provide a web-based, mobile-responsive interface. | Project context / PROPOSAL | Must | Core workflows are usable on agreed desktop and mobile viewport/device profiles. | PROPOSAL |
| NFR-002 | Use Amharic as the primary interface language and support English. | Project context / PROPOSAL | Must | Core screens, validation, notifications and reports have reviewed Amharic and English strings; text renders and searches correctly. | PROPOSAL |
| NFR-003 | Use ETB as the initial currency. | Project context / PROPOSAL | Must | Financial display and reports use ETB with consistent precision and formatting; accounting policy is confirmed. | PROPOSAL |
| NFR-004 | Assess intermittent-connectivity and offline-tolerant workflows. | Project context / PROPOSAL | Should | A documented connectivity assessment identifies offline use cases, sync conflict policy and security boundaries; no offline feature is assumed implemented. | UNRESOLVED |
| NFR-005 | Define measurable performance, availability, capacity and growth targets. | Architecture assessment | Must | Targets are based on verified user/device/connectivity estimates and are testable; current estimates are not treated as measured demand. | UNRESOLVED |
| NFR-006 | Evaluate hosting, portability, maintenance cost and local supportability before selecting technology. | Architecture assessment | Must | Options matrix compares total cost, skills, security support, backup, connectivity, portability and operational burden. | UNRESOLVED |
| NFR-007 | Assess accessibility, including WCAG 2.2 AA as a proposed target. | A1 proposal | Should | Accessibility target is approved and key flows are evaluated using documented tests. | PROPOSAL |

## 6. Stakeholder and responsibility model — preliminary

| Stakeholder | Candidate responsibilities | Authority status |
|---|---|---|
| Church Owner / governing authority | Institutional ownership, governance and delegated policy | Owner-approved institutional basis recorded under OD-RSMS-008; individual role/delegation limits remain unresolved |
| School leadership | Daily school administration and operational oversight | Exact roles and delegations TBD |
| Academic leadership | Calendar, curriculum, assessment and promotion oversight | TBD |
| Registrar / admissions | Student records, enrollment and transfers | Candidate role only |
| Teachers | Assigned class attendance and academic records | Candidate role only |
| Finance officer | Fee schedules, ledgers, reconciliation and finance reporting | Candidate role only |
| Cashier | Cash receipt issuance and cash custody | Assignment and custody policy TBD |
| Budget/expense approvers | Review and approval within delegated limits | Must not be configured until approved authority matrix exists |
| System administrator | Technical configuration, access administration and support | No implied financial approval authority |
| Parents/guardians | Access to authorized linked student information | Identity verification and access policy TBD |
| Auditor/reviewer | Read-only oversight according to approved mandate | Mandate and scope TBD |

This is a discovery model, not an approved organization chart or delegation of authority.

## 7. Core workflow outlines — preliminary

### 7.1 Student admission and enrollment
Application/record intake → identity and supporting-document checks → authorized admission decision → student identifier assignment → grade/section placement → enrollment confirmation. Exception handling, required documents, admission authority and retention rules require school validation.

### 7.2 Semester academic cycle
Configure academic year and two semesters → configure grades/sections/subjects → assign teachers and students → record attendance and assessments → review/approve marks → issue reports → authorized promotion/repetition decision → preserve historical records. Dates, grading and approval roles remain unresolved.

### 7.3 Cash fee collection
Verify student/account and approved charge → receive cash → issue unique receipt → post transaction to student account → reconcile cashier session and receipt sequence → review variances → close daily collection. Cash custody, cashier assignment, receipt book controls, reversal authority and reconciliation sign-off require Owner-approved procedures.

### 7.4 Budget and major expense
Requester submits purpose, category, amount and supporting evidence → delegated reviewer checks completeness/budget → authorized approver decides within threshold → payment is executed by a separate authorized role where feasible → transaction is recorded and reconciled → audit trail retained. This workflow is conceptual only; no thresholds or roles may be inferred.

## 8. Non-functional and assurance questions still open

- Expected concurrent users, student count, annual growth and device mix.
- Connectivity, electricity and device availability at school.
- Hosting location, data residency, vendor access and operating costs.
- Recovery point and recovery time objectives.
- Record retention, archival, correction and deletion rules.
- Applicable Ethiopian education, child protection, privacy/data protection, employment, tax and financial obligations.
- Accessibility target and testing responsibility.
- Support ownership, training, change management and operational handover.

## 9. Traceability and change control

- Requirement IDs are stable; do not reuse retired IDs.
- Every requirement must cite an Owner decision, institutional evidence, stakeholder-confirmed need or clearly labelled proposal.
- A requirement is not approved merely because it appears in this register.
- Changes require a dated rationale, source, impact assessment and approval record.
- A2 must reconcile this register against available evidence and actual workflows without modifying production systems; do not request further institutional documents from the Owner.
- A1 approval requires explicit Owner approval of a versioned baseline; this register remains preliminary until then.

## 10. A1 gap summary

**Critical unresolved:** Academy-specific school registration/licensing/accreditation status under Proclamation 1368/2025; internal role assignments and delegations; budget/expense approval matrix; tuition/fee schedules; cashier assignment, cash custody and reconciliation; student-data privacy/retention design and qualified legal review. The Church institutional-authority basis is Owner-dispositioned under OD-RSMS-008.

**Other unresolved:** academic calendar dates, KG structure, sections, subjects, grading, promotion rules, staffing, devices/connectivity, technology/hosting options, capacity targets, backup/recovery and support model.

**Disposition:** PARTIAL. This register improves traceability but does not complete A1 or authorize A2/A3.
