# Master Business Functions Index

In C50's operating model, running a specialized **Databricks** and cloud data engineering firm organizes around eight core business functions. Delivery and Resource/Capacity Management are combined into a single function (**Function 03**) to keep commercial commitments, technical execution, and staffing aligned.

---

## 8-Function Status

| # | Business Function | Category | What It Covers | Primary Owner (20 People) | Primary KPI | Status | Detailed Design Doc |
| :-: | :--- | :--- | :--- | :--- | :--- | :---: | :--- |
| **01** | **Partner Alliances & Sales** | Core Revenue | Selling through Databricks and cloud partner relationships; architecture audits | Alliance Lead / Principals | 50%–60% partner-sourced pipeline | `Pending` | `docs/operating_model/functions/01_partner_alliances_and_sales.md` |
| **02** | **Marketing & Brand Positioning** | Core Revenue | Inbound technical content, partner MDF funding, cloud marketplace listings | Marketing Specialist / Ops | Lead conversion & MDF funds claimed | `Pending` | `docs/operating_model/functions/02_marketing_and_ecosystem.md` |
| **03** | **Delivery, Resource & Capacity Management** | Delivery Execution | Pod-based delivery, skill-based assignment, capacity planning, bench management | Principal Data Architects & Delivery Mgr | Utilization $\ge 75\%$; Margin $>50\%$; Bench $<8\%$ | `IN_DESIGN` | [`03_delivery_resource_and_capacity_management.md`](file:///Users/jason/C50%20Project/docs/operating_model/deep_dives/03_delivery_resource_and_capacity_management.md) |
| **04** | **Finance, Accounting & FinOps** | Enabling | Project billing, DSO management, cloud vendor credits, FinOps gain-share accounting | Operations & Finance Lead | DSO $<45$ days; gross margin tracking | `Pending` | `docs/operating_model/functions/05_finance_accounting_and_finops.md` |
| **05** | **Talent Operations & Recruiting** | Enabling | Specialized sourcing & vetting for Analytics & Data Engineers; retention & compensation | Technical Recruiter & Ops | Time-to-hire $<30$ days; offer acceptance rate | `Pending` | `docs/operating_model/functions/06_talent_operations_and_recruiting.md` |
| **06** | **Legal, Security & Risk Governance** | Enabling | MSAs/SOWs, PII masking, cloud cost overrun liability clauses, SOC 2 Type II, HIPAA | Principals (Ext. Legal) | Zero compliance violations; clean audit | `Pending` | `docs/operating_model/functions/07_legal_security_and_risk.md` |
| **07** | **Tooling, Sandbox & IT Ops** | Enabling | Developer tools, cloud sandbox credits, CI/CD runners, data observability | DataOps & FinOps Lead | Tooling cost per person; sandbox uptime | `Pending` | `docs/operating_model/functions/08_tooling_sandbox_and_it_ops.md` |
| **08** | **Practice Dev & IP Accelerators** | Enabling | Reusable lakehouse templates, IaC libraries, migration tools, industry data models | Principal Data Architects | Asset reuse rate (40% setup time reduction) | `Pending` | `docs/operating_model/functions/09_practice_dev_and_ip_accelerators.md` |

---

## How the Functions Work Together

```
                                      +-------------------------------+
                                      | 01. Partner Alliances & Sales |
                                      +---------------+---------------+
                                                      |
                                                      v
  +--------------------------------+  +---------------+---------------+  +--------------------------------+
  | 02. Marketing & Brand          |->| 03. Delivery, Resource        |<-| 05. Talent Operations          |
  |    (MDF & Partner Co-branding) |  |     & Capacity Management     |  |    (Specialized Data Profiles) |
  +--------------------------------+  +---------------+---------------+  +--------------------------------+
                                                      |
                                                      v
  +--------------------------------+  +---------------+---------------+  +--------------------------------+
  | 04. Finance, Acct & FinOps     |<-| 06. Legal, Risk & Governance  |->| 08. Practice Dev & IP Lab      |
  |    (Margin & Gain-share Calc)  |  |    (SOWs & Data Liability)    |  |    (IaC & Code Libraries)      |
  +--------------------------------+  +-------------------------------+  +--------------------------------+
                                                      |
                                                      v
                                      +-------------------------------+
                                      | 07. Tooling & Cloud Sandboxes |
                                      +-------------------------------+
```
