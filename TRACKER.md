# Consulting 5.0 (C50) — Master Functional Area Tracker

> **Project Mission:** Build and grow a specialized **Databricks** data engineering firm from 20 people to 100, maintaining $\ge 55\%$ gross margins and results-based contracts.

---

## 📊 Master Functional Dashboard

| # | Business Functional Area | Category | Primary Owner (20 People) | Target KPI | Design Status | Progress |
| :-: | :--- | :--- | :--- | :--- | :---: | :---: |
| **01** | **Partner Alliances & Channel Sales** | Core Revenue | Alliance & Channel Sales Lead | 50%–60% partner-sourced pipeline | `BACKLOG` | 15% |
| **02** | **Marketing & Brand Positioning** | Core Revenue | Marketing Specialist / Operations | 100% MDF claimed; inbound deal flow | `BACKLOG` | 15% |
| **03** | **Delivery, Resource & Capacity Management** | Delivery Execution | Principal Data Architects & Data Delivery Mgr | Utilization $\ge 75\%$; Margin $>50\%$; Unassigned time $<8\%$ | `IN_DESIGN` | 75% |
| **04** | **Finance, Accounting & FinOps** | Operational Enabling | Operations & Finance Lead | DSO $<45$ days; accurate gain-share calc | `BACKLOG` | 15% |
| **05** | **Talent Operations & Recruiting** | Operational Enabling | Technical Recruiter & People Ops | Time-to-hire $<30$ days; offer accept $>85\%$ | `BACKLOG` | 15% |
| **06** | **Legal, Security & Risk Governance** | Operational Enabling | Principal Data Architects (Ext. Legal) | Zero compliance breaches; clean SOC 2 | `BACKLOG` | 15% |
| **07** | **Tooling, Sandbox & IT Ops** | Operational Enabling | DataOps & FinOps Lead | Tooling cost $< \$600/\text{person/mo}$; 99.9% uptime | `BACKLOG` | 15% |
| **08** | **Practice Dev & IP Accelerators** | Enterprise Value | Principal Data Architects | $40\%$ initial setup time reduction | `BACKLOG` | 15% |

---

## 📐 8-Part Functional Design Checklist

Every functional area design must cover all 8 areas:

1. **Purpose & Scope:** Why this function exists, what it owns, and what it doesn't.
2. **Team Structure & Roles:** Headcount, job descriptions, utilization expectations, and responsibility assignment (RACI).
3. **How It Operates Day-to-Day:** Detailed workflows, step-by-step processes, inputs, and outputs.
4. **Commercial & Financial Mechanics:** Budget, cost center, unit economics, and margin contribution.
5. **Metrics & Escalation Rules:** Primary KPI, secondary operational metrics, and when to escalate.
6. **Tools & Systems:** Software categories, platform tiers, and access control policies.
7. **Templates & Assets:** Standard contracts, SOW clauses, runbooks, intake forms, checklists.
8. **Growth Plan (20 → 60 → 100 People):** Trigger points, team splits, and automation upgrades across growth phases.

---

## 🔄 Cross-Functional Dependencies

```
                                  +------------------------------------+
                                  | 01. Partner Alliances & Sales      |
                                  | (Databricks, Cloud Partners)       |
                                  +-----------------+------------------+
                                                    |
                                      Pipeline & SOWs|
                                                    v
  +--------------------------------+      +---------+--------------------------+      +--------------------------------+
  | 02. Marketing & Brand          | ---> | 03. Delivery, Resource & Capacity  | <--- | 05. Talent Operations          |
  | (MDF, Case Studies, Brand)     |      |     Management (Delivery Pods)     |      | (Specialized Tech Recruiting)  |
  +--------------------------------+      +---------+--------------------------+      +--------------------------------+
                                                    |
                                      Reusable IP & | Revenue & Cloud Data
                                      Margin Data   v
  +--------------------------------+      +---------+--------------------------+      +--------------------------------+
  | 08. Practice Dev & IP Lab      | <--- | 04. Finance, Accounting & FinOps   | ---> | 06. Legal, Security & Risk     |
  | (IaC Templates & Libraries)    |      | (Gain-share, Billing, Margin QA)   |      | (DoD Contracts, Liability Caps)|
  +--------------------------------+      +------------------------------------+      +--------------------------------+
                                                    |
                                        Tooling & Ops|
                                                    v
                                  +------------------------------------+
                                  | 07. Tooling, Sandboxes & IT Ops    |
                                  | (Multi-Cloud Credits, CI/CD, MDM)  |
                                  +------------------------------------+
```

---

## 📋 Functional Area Workstream Status

### 01. Partner Alliances & Channel Sales
* **Category:** Core Revenue
* **Lead:** Alliance & Channel Sales Lead (supported by Principal Architects)
* **Status:** `BACKLOG`
* **File:** [`01_partner_alliances_and_sales.md`](file:///Users/jason/C50%20Project/docs/operating_model/functions/01_partner_alliances_and_sales.md)
* **Required Blueprint Deliverables:**
  - [ ] Platform partner tier progression roadmap (Databricks, AWS, GCP, Azure).
  - [ ] Partner Account Manager (PAM) and field Account Executive (AE) joint selling playbook.
  - [ ] Deal registration workflow, CRM integration, and attribution tracking.
  - [ ] Fixed-fee discovery engagement conversion framework (\$25k–\$45k audit $\rightarrow$ multi-sprint delivery).
  - [ ] Cloud Marketplace transaction strategy (Customer Partner Private Offers).

### 02. Marketing & Brand Positioning
* **Category:** Core Revenue
* **Lead:** Marketing Specialist (supported by Operations Lead)
* **Status:** `BACKLOG`
* **File:** [`02_marketing_and_ecosystem.md`](file:///Users/jason/C50%20Project/docs/operating_model/functions/02_marketing_and_ecosystem.md)
* **Required Blueprint Deliverables:**
  - [ ] Partner MDF (Market Development Funds) capture and deployment SOP.
  - [ ] Technical case study production process (quantified business ROI).
  - [ ] Technical content calendar (bi-weekly deep dives, industry comparison reports).
  - [ ] Partner conference event strategy (Databricks Data+AI Summit, cloud partner summits).
  - [ ] Inbound lead scoring and qualification process for high-value enterprise accounts.

### 03. Delivery, Resource & Capacity Management
* **Category:** Delivery Execution
* **Lead:** Principal Data Architects & Data Delivery Manager
* **Status:** `IN_DESIGN` (Foundation captured, interactive microsite created, completing full 8-part operational design & execution plan)
* **File:** [`03_delivery_resource_and_capacity_management.md`](file:///Users/jason/C50%20Project/docs/operating_model/deep_dives/03_delivery_resource_and_capacity_management.md)
* **Interactive Microsite:** [`index.html`](file:///Users/jason/C50%20Project/docs/operating_model/microsites/delivery_resource_governance/index.html)
* **8-Part Design Checklist:**
  - [x] **Part 1:** Purpose & Scope (Pod-based execution, outcome delivery).
  - [x] **Part 2:** Team Structure & Roles (Pod composition, utilization benchmarks, leadership split).
  - [x] **Part 3:** Detailed Operating Cadences & SOPs (Intake, sprint rituals, QA gateways, handoff & offboarding SOPs).
  - [x] **Part 4:** Commercial & Financial Mechanics (Pod sprint economics, margin protection, scope change pricing).
  - [x] **Part 5:** Metrics & Escalation Rules (Utilization $\ge 75\%$, Margin $\ge 55\%$, Unassigned time $<8\%$, escalation triggers).
  - [x] **Part 6:** Tools & Systems (PSA / Resource Management, Issue Tracker, Project Accounting, Code Repository / CI/CD, Data Transformation & Observability).
  - [x] **Part 7:** Templates & Assets (Pod Sprint Planner, Skill Matrix Rubric, QA Sign-off Sheet, DoD Checklist).
  - [x] **Part 8:** Growth Plan (Trigger points at 35, 60, and 100 people).

### 04. Finance, Accounting & FinOps
* **Category:** Operational Enabling
* **Lead:** Operations & Finance Lead
* **Status:** `BACKLOG`
* **File:** [`05_finance_accounting_and_finops.md`](file:///Users/jason/C50%20Project/docs/operating_model/functions/05_finance_accounting_and_finops.md)
* **Required Blueprint Deliverables:**
  - [ ] Outcome-based milestone billing & revenue recognition schedule.
  - [ ] Fully loaded pod sprint costing model and real-time margin tracking dashboard.
  - [ ] FinOps gain-share calculation, baseline metering, and audit verification process.
  - [ ] Working capital and Days Sales Outstanding (DSO) management playbooks ($<45$ days).
  - [ ] Partner cloud credit drawdown and consumption monitoring.

### 05. Talent Operations & Technical Recruiting
* **Category:** Operational Enabling
* **Lead:** Technical Recruiter & People Ops
* **Status:** `BACKLOG`
* **File:** [`06_talent_operations_and_recruiting.md`](file:///Users/jason/C50%20Project/docs/operating_model/functions/06_talent_operations_and_recruiting.md)
* **Required Blueprint Deliverables:**
  - [ ] Specialized role profiles & skill rubrics (Analytics Engineer, Spark/Databricks Data Engineer, DataOps/FinOps).
  - [ ] 3-stage practical technical evaluation process (hands-on code challenges vs whiteboard).
  - [ ] Compensation bands, billable utilization targets, and pod margin bonus pool design.
  - [ ] Onboarding curriculum (standard 10-day ramp to pod billable readiness).
  - [ ] On-demand 1099 contractor management process.

### 06. Legal, Security & Risk Governance
* **Category:** Operational Enabling
* **Lead:** Principal Data Architects (Supported by External Legal Counsel)
* **Status:** `BACKLOG`
* **File:** [`07_legal_security_and_risk.md`](file:///Users/jason/C50%20Project/docs/operating_model/functions/07_legal_security_and_risk.md)
* **Required Blueprint Deliverables:**
  - [ ] Outcome-based Master Services Agreement (MSA) and Statement of Work (SOW) templates.
  - [ ] Cloud compute cost overrun liability caps and disclaimer clauses.
  - [ ] Data security, PII masking, and zero-client-data-at-rest policies.
  - [ ] SOC 2 Type II readiness and HIPAA business associate compliance framework.
  - [ ] IP ownership boundaries (reusable firm IP vs client-specific schema/models).

### 07. Tooling, Sandbox & IT Ops
* **Category:** Operational Enabling
* **Lead:** DataOps & FinOps Lead
* **Status:** `BACKLOG`
* **File:** [`08_tooling_sandbox_and_it_ops.md`](file:///Users/jason/C50%20Project/docs/operating_model/functions/08_tooling_sandbox_and_it_ops.md)
* **Required Blueprint Deliverables:**
  - [ ] Production software catalog and per-seat SaaS budget management ($< \$600/\text{person/mo}$).
  - [ ] Multi-cloud sandbox setup (isolated AWS, Azure, GCP accounts with budget kill-switches).
  - [ ] Central identity, access management (IdP/SSO), and credentials management.
  - [ ] Automated engineer workstation provisioning via Mobile Device Management (MDM).
  - [ ] Observability, CI/CD runners, and automated data testing infrastructure.

### 08. Practice Development & IP Accelerators
* **Category:** Enterprise Value
* **Lead:** Principal Data Architects
* **Status:** `BACKLOG`
* **File:** [`09_practice_dev_and_ip_accelerators.md`](file:///Users/jason/C50%20Project/docs/operating_model/functions/09_practice_dev_and_ip_accelerators.md)
* **Required Blueprint Deliverables:**
  - [ ] Reusable asset capture workflow from completed sprint deliverables.
  - [ ] Core codebase libraries (Terraform multi-cloud lakehouse, standard transformation project templates).
  - [ ] Industry vertical data models (Healthcare FHIR, Retail Customer 360, FinTech Fraud).
  - [ ] Unassigned-time playbook (redirecting unassigned hours into IP assets).
  - [ ] IP review and sanitization process (ensuring zero proprietary client logic leaks into firm assets).

---

## 🗓️ Recommended Execution Order

```
[Phase 1: Delivery Core]
  ★ Function 03: Delivery, Resource & Capacity Management (IN DESIGN)
        │
        ▼
[Phase 2: Revenue Engine]
  1. Function 01: Partner Alliances & Channel Sales
  2. Function 02: Marketing & Brand Positioning
        │
        ▼
[Phase 3: Financial & Legal]
  3. Function 04: Finance, Accounting & FinOps
  4. Function 06: Legal, Security & Risk Governance
        │
        ▼
[Phase 4: Talent & Infrastructure]
  5. Function 05: Talent Operations & Technical Recruiting
  6. Function 07: Tooling, Sandbox & IT Ops
        │
        ▼
[Phase 5: Long-Term Value]
  7. Function 08: Practice Development & IP Accelerators
```
