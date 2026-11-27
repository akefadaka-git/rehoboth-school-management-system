# A1 Open Decisions and Evidence Resolution Register

**Artifact:** R-SMS-A1-RES-001  
**Version:** 0.1 — review working register  
**Date:** 27 November 2026  
**Project:** Rehoboth Academy School Management System (R-SMS)  
**Status:** OPEN — working register; not an approved policy or A1 freeze  
**Branch:** `docs/a1-review-mainline`

## 1. Purpose and control

This register converts the remaining A1 institutional and operational gaps into explicit resolution items. It distinguishes:

- **OWNER-RECORDED:** a decision explicitly supplied by the Owner.
- **EVIDENCE REQUIRED:** an existing institutional fact or rule must be supported by an authoritative record.
- **OWNER DECISION REQUIRED:** the institution must choose or approve a policy, role, threshold or operating rule.
- **STAKEHOLDER VALIDATION REQUIRED:** the current workflow or practical constraint must be confirmed by the people performing it.
- **PROPOSED CONTROL:** a recommended system/control behavior, not an adopted school policy.
- **BLOCKED:** cannot be closed from available evidence.

No blank is to be completed by inference. Where an institutional document does not exist, record that fact and obtain an explicit Owner decision on the interim policy and its authority. Sensitive source documents must not be committed to this public repository; record only document title/type, issuing authority, date, version, verification outcome and a restricted evidence location/reference.

## 2. Already established Owner decisions

| ID | Confirmed direction | A1 treatment |
|---|---|---|
| OD-RSMS-001 | Koibe Kale Hiwot Church owns and operates Rehoboth Academy. | Owner-provided; supporting registration/governance records still required. |
| OD-RSMS-002 | Budget and major expenses use a shared approval policy. | Policy direction confirmed; roles, limits and workflow remain open. |
| OD-RSMS-003 | Academy offers Kindergarten and Grades 1–6. | Scope confirmed; KG levels, grade naming and sections remain open. |
| OD-RSMS-004 | Academic year has two semesters. | Structure confirmed; calendar dates and academic rules remain open. |
| OD-RSMS-005 | School fees are currently collected in cash only. | Current-state confirmed; cashier and cash controls remain open. |
| OD-RSMS-006 | Repository remains Public during development and becomes Private only after deployment. | Active repository instruction; no change before post-deployment gate. |
| OD-RSMS-007 | Independent review is not required at any R-SMS stage. | Owner approval governs project decisions; GitHub technical permissions remain separate. |

## 3. Institutional authority and governance

| ID | Resolution item | Required input/evidence | Closure test | Status |
|---|---|---|---|---|
| INST-01 | Confirm legal identity and registration of Koibe Kale Hiwot Church. | Registration certificate or authoritative registration record; issuer, number, date and current status. | Issuer and validity are checked; evidence reference is recorded without publishing sensitive scans. | BLOCKED — EVIDENCE REQUIRED |
| INST-02 | Confirm legal/administrative status of Rehoboth Academy and its authority to operate. | School registration/license/approval, if applicable; issuing authority and validity. | Status and scope of authorization are recorded; any missing approval is explicit. | BLOCKED — EVIDENCE REQUIRED |
| INST-03 | Confirm governing body and its powers. | Church constitution/bylaws, governing rules, minutes or equivalent authoritative instrument. | Governing body, appointment method, quorum/decision rules and relevant powers are mapped. | BLOCKED — EVIDENCE REQUIRED |
| INST-04 | Identify named school leadership roles and reporting lines. | Current approved organization chart or Owner-confirmed role list. | Each operational role has a named position (not necessarily a personal name), supervisor and delegated responsibilities. | BLOCKED — OWNER INPUT |
| INST-05 | Define delegated authority and signing powers. | Approved delegation/authority matrix or explicit Owner-approved interim matrix. | Each decision type has an accountable authority, delegate, limit, substitute and evidence requirement. | BLOCKED — OWNER DECISION |
| INST-06 | Define who may approve policies and changes to school rules. | Governing instrument and Owner direction. | Policy approval, operational procedure approval and system configuration authority are distinguished. | BLOCKED — OWNER INPUT / EVIDENCE |

## 4. Budget and major-expense approval

The shared approval direction is recorded. The following details must be explicitly settled before finance workflow requirements can be frozen:

| ID | Resolution item | Required decision | Closure test | Status |
|---|---|---|---|---|
| FIN-GOV-01 | Define what counts as a major expense. | Amount threshold, category-based definition, or both; currency ETB. | A clear rule distinguishes routine expenses from major expenses. | BLOCKED — OWNER DECISION |
| FIN-GOV-02 | Define budget preparation and approval. | Who prepares, reviews, recommends and finally approves the annual/term budget. | Each stage and approving authority is identified. | BLOCKED — OWNER DECISION |
| FIN-GOV-03 | Define expense request approval levels. | Requester, budget checker, reviewer, approver and payment executor roles. | A role/authority matrix exists; no person approves their own request or payment without an explicitly approved exception. | BLOCKED — OWNER DECISION |
| FIN-GOV-04 | Define monetary approval bands. | ETB ranges and required approval combination for each band. | Every amount falls into a defined band; no overlapping or uncovered ranges. | BLOCKED — OWNER DECISION |
| FIN-GOV-05 | Define unbudgeted/emergency expense treatment. | Emergency definition, interim limit, notification and retrospective ratification authority/time limit. | Emergency path is bounded, documented and auditable. | BLOCKED — OWNER DECISION |
| FIN-GOV-06 | Define payment execution and custody separation. | Who authorizes, releases, pays, receives and reconciles funds. | Request, approval, payment and reconciliation duties are separated where practicable; exceptions are documented. | BLOCKED — OWNER DECISION |
| FIN-GOV-07 | Define procurement evidence. | Quotations, invoices, purchase orders, receiving confirmation and exception rules. | Required supporting documents are specified by expense type/threshold. | BLOCKED — STAKEHOLDER / OWNER INPUT |

**Proposed system control (not yet adopted policy):** enforce maker-checker separation; block self-approval; require supporting evidence; retain approval history; prevent approval above delegated limits; route unbudgeted/emergency requests through a separately authorized path; and use reversal/adjustment records rather than deleting posted transactions.

## 5. Cash fee collection and reconciliation

| ID | Resolution item | Required decision / evidence | Closure test | Status |
|---|---|---|---|---|
| CASH-01 | Identify cashier position(s) and authorized substitutes. | Current assignment/appointment and who authorizes changes. | Cashier and substitute authorization are recorded by role and effective date. | BLOCKED — OWNER INPUT |
| CASH-02 | Define cash custody. | Where cash is held, who has keys/access, transfer process and deposit frequency, if any. | Custody, handover and access responsibilities are explicit. | BLOCKED — STAKEHOLDER / OWNER INPUT |
| CASH-03 | Define receipt numbering. | Existing receipt books/sequence, prefix/year rules, duplicate/lost/void handling. | Number uniqueness and sequence custody are defined across paper and future system records. | BLOCKED — EVIDENCE / OWNER INPUT |
| CASH-04 | Define daily close and reconciliation. | Cashier count, receipt register, student ledger comparison, reviewer and sign-off. | Daily totals reconcile; variances are documented, reviewed and escalated. | BLOCKED — OWNER INPUT |
| CASH-05 | Define refunds, corrections and reversals. | Who authorizes refunds, cancelled receipts, mistaken payments and balance corrections. | Original transaction remains traceable; approval and reason are recorded. | BLOCKED — OWNER DECISION |
| CASH-06 | Define fee schedule and due dates. | Approved registration, tuition, recurring and other fee schedule; discounts/waivers/late fees, if any. | Every charge has approved amount, applicability, effective dates and authorizing source. | BLOCKED — EVIDENCE / OWNER DECISION |
| CASH-07 | Define receipt content and payer identity. | Required student/payer details and acceptable proof of payment. | Receipt fields and duplicate-payment checks are agreed. | BLOCKED — STAKEHOLDER INPUT |
| CASH-08 | Define arrears and hardship handling. | Due dates, installment rules, waiver authority, reminders and escalation. | Balance treatment and exceptions are approved; no automatic penalty is assumed. | BLOCKED — OWNER DECISION |

**Proposed minimum cash workflow (subject to validation):** verify student and approved charge → receive ETB cash → issue controlled sequential receipt → post payment once to student ledger → provide payer receipt → close cashier session → compare cash counted, receipt sequence and ledger postings → record variance → independent authorized review of the close. “Independent review” here means an internal second-person cash reconciliation control, not an external project reviewer; the institution must decide whether and how this control is operationally feasible.

## 6. Academic and student operations

| ID | Resolution item | Required decision / evidence | Closure test | Status |
|---|---|---|---|---|
| ACAD-01 | Define KG structure. | KG level names and progression (e.g., levels actually offered). | Exact class names and sequence are confirmed by school leadership. | BLOCKED — OWNER / ACADEMIC INPUT |
| ACAD-02 | Confirm grade/section naming and capacity. | Section names, class-size limits and whether parallel sections exist. | Grade-section catalogue and capacity rules are documented. | BLOCKED — ACADEMIC INPUT |
| ACAD-03 | Define academic year dates and semester dates. | Start/end dates, holidays, enrollment cutoffs and calendar authority. | Calendar is versioned and approved for the relevant year. | BLOCKED — OWNER / ACADEMIC INPUT |
| ACAD-04 | Confirm calendar convention. | Ethiopian calendar, Gregorian calendar or dual display; date authority and conversion rules. | Authoritative date examples are tested and accepted. | BLOCKED — OWNER DECISION |
| ACAD-05 | Define curriculum and subject catalogue. | Approved grade-wise subjects and subject naming. | Subject list and grade applicability are recorded. | BLOCKED — ACADEMIC EVIDENCE |
| ACAD-06 | Define assessment and grading. | Assessment types, weights, grading scale, pass marks, rounding and report format. | Calculations are reproducible from approved policy and sample cases. | BLOCKED — OWNER / ACADEMIC DECISION |
| ACAD-07 | Define promotion, repetition and completion. | Decision authority, minimum criteria, exceptions and appeal/correction process. | Each progression outcome has approved criteria and recorded decision authority. | BLOCKED — OWNER / ACADEMIC DECISION |
| ACAD-08 | Define admission, transfer and withdrawal. | Required documents, admission authority, transfer records and withdrawal process. | Lifecycle workflows and record retention are agreed. | BLOCKED — SCHOOL INPUT |
| ACAD-09 | Define attendance and discipline. | Attendance codes, lateness/absence rules, correction authority and discipline process. | Codes, workflows and restricted access are documented. | BLOCKED — SCHOOL INPUT |
| ACAD-10 | Define parent/guardian access. | Identity verification, linked-student access, consent/authority and dispute process. | A guardian can only access records for a verified authorized relationship. | BLOCKED — OWNER / PRIVACY INPUT |

## 7. People, payroll and accounting scope

| ID | Resolution item | Required input | Closure test | Status |
|---|---|---|---|---|
| HR-01 | Confirm staff categories and employment records needed. | Staff list by position/category (avoid publishing personal data); employment record fields and custodian. | Required HR scope and access boundaries are specified. | BLOCKED — SCHOOL INPUT |
| HR-02 | Confirm payroll scope. | Whether the school requires payroll calculation, payslip, deductions, tax/statutory reporting or only staff payment records. | Payroll scope and applicable accounting/legal requirements are explicitly determined. | BLOCKED — OWNER / FINANCE INPUT |
| FIN-08 | Confirm accounting scope. | Cashbook only, income/expense ledger, full double-entry accounting, budget reports, financial statements or other. | Required accounting outputs and reporting periods are listed. | BLOCKED — OWNER / FINANCE INPUT |
| FIN-09 | Confirm chart of accounts and fiscal periods. | Existing books, account categories and year-end rules. | Approved account structure and period close rules are documented. | BLOCKED — FINANCE EVIDENCE |

## 8. Privacy, legal and records

| ID | Resolution item | Required input/evidence | Closure test | Status |
|---|---|---|---|---|
| PRIV-01 | Identify applicable institutional and statutory obligations. | School registration/approval conditions and qualified Ethiopian legal/regulatory review. | Obligations register identifies source, applicability, responsible role and compliance evidence. | BLOCKED — QUALIFIED REVIEW |
| PRIV-02 | Define student/child data handling. | Data categories, purpose, access, guardian authority, disclosure and correction process. | Data inventory and access matrix are approved. | BLOCKED — OWNER / QUALIFIED REVIEW |
| PRIV-03 | Define retention and disposal. | Retention periods for student, academic, finance, HR and correspondence records; archival and disposal authority. | Each record class has retention trigger, period, hold and disposal rule. | BLOCKED — OWNER / QUALIFIED REVIEW |
| PRIV-04 | Define incident handling. | Responsible role, reporting route, containment and notification decision authority. | Incident procedure and escalation contacts are documented in restricted records. | BLOCKED — OWNER INPUT |
| PRIV-05 | Confirm repository/publication boundary. | Public documentation review and data classification rules. | No real student, parent, staff, credential, account or confidential records are committed to the public repository. | ACTIVE CONTROL — CONTINUOUS |

## 9. Technology and operating environment

| ID | Resolution item | Required input/evidence | Closure test | Status |
|---|---|---|---|---|
| TECH-01 | Measure student/staff/user scale and peak concurrency. | Current counts by role and expected growth. | Baseline is sourced and distinguishes measured facts from estimates. | BLOCKED — SCHOOL INPUT |
| TECH-02 | Assess devices, power and connectivity at school. | Device inventory, network reliability, power interruptions and available support. | Site assessment records actual constraints and representative usage. | BLOCKED — SITE ASSESSMENT |
| TECH-03 | Evaluate technology and hosting options. | Locally supportable options, lifecycle/security support, data location, total cost and vendor access. | Options matrix and cost assumptions are documented; no paid commitment is made. | BLOCKED — A1 ANALYSIS |
| TECH-04 | Set backup and recovery objectives. | Acceptable data loss (RPO), restoration time (RTO), backup frequency and custodian. | Objectives are approved and a future restore test is specified. | BLOCKED — OWNER / TECHNICAL INPUT |
| TECH-05 | Prioritize offline workflows. | Which roles/tasks must work during connectivity loss and what devices are available. | Offline requirements, sync conflicts and security limits are specified or offline is explicitly deferred. | BLOCKED — SCHOOL INPUT |
| TECH-06 | Define training and support. | Who administers, trains users, handles incidents and maintains records. | Operating ownership, support route and handover criteria are recorded. | BLOCKED — OWNER INPUT |
| TECH-07 | Set measurable service targets. | Availability, response time, supported devices/browsers and peak use assumptions. | Targets are realistic, measurable and tied to an operating model. | BLOCKED — A1 ANALYSIS |

## 10. A1 resolution order

1. **Institutional authority:** INST-01 to INST-06.
2. **Financial authority and cash controls:** FIN-GOV-01 to FIN-GOV-07 and CASH-01 to CASH-08.
3. **Academic operating rules:** ACAD-01 to ACAD-10.
4. **People, accounting and privacy:** HR-01 to HR-02, FIN-08 to FIN-09 and PRIV-01 to PRIV-05.
5. **Technology and operating feasibility:** TECH-01 to TECH-07.

An item may be closed only with one of: (a) verified authoritative evidence; (b) an explicit Owner decision; (c) documented stakeholder validation where the matter is an observed workflow; or (d) an explicit decision to defer/exclude the capability from initial scope. Deferral must include rationale, impact and responsible authority. “Not known” is a valid recorded outcome; it is not a resolved requirement.

## 11. A1 exit control

A1 cannot be submitted for freeze while critical institutional authority, financial approval, cash custody/reconciliation, academic rules, privacy/retention and technology feasibility are represented as silently resolved. Any residual open item must be listed with impact and either resolved or explicitly accepted/deferred by the authority entitled to do so.

This register does not authorize A2, A3, expenditure, production data import, deployment or merge. It is a working A1 review artifact on the existing documentation branch.
