# 3. How We Price Work

## The Problem with the Billable Hour

Traditional consulting has a built-in contradiction: if a firm works faster and builds reusable tools, it bills fewer hours and earns less revenue.

**C50 prices by result, not by time.** Each engagement is scoped to a clear Definition of Done (DoD) — a specific, agreed list of what "done" looks like — with predictable pod sprint costs and margin targets ($\ge 55\%$).

```
       OLD MODEL (T&M / Hourly Billing)                  NEW MODEL (Outcome-Based / Pod Pricing)
+-----------------------------------------------+   +-----------------------------------------------+
| • Track 80% billable hours per consultant     |   | • Track Pod Sprint Velocity & Milestone QA    |
| • Argue over timesheet entries & code billing |   | • Track Project Gross Margin per Pod          |
| • Client pays for time, regardless of speed   |   | • Client pays for completed Definition of Done|
| • Margin drops if team works too fast         |   | • Margin INCREASES if team works faster/better|
+-----------------------------------------------+   +-----------------------------------------------+
```

---

## Outcome Packages

| Package | Deliverable & Definition of Done (DoD) | Commercial Structure | Target Price Range |
| :--- | :--- | :--- | :--- |
| **1. Databricks Architecture Audit & Blueprint** | Production-ready lakehouse design, Unity Catalog security/governance policy, data lineage map, and 90-day technical execution roadmap. | Fixed-Fee Discovery | \$25,000 – \$45,000 |
| **2. Lakehouse Migration & Foundation** | Ingestion pipeline deployment, transformation modeling layers, 100% passing automated test suite (schema & data quality), and fully automated CI/CD deployment. | Milestone-Based Outcome (3–5 Sprints) | \$120,000 – \$250,000 |
| **3. FinOps Cloud Compute Optimization** | Comprehensive optimization of lakehouse compute/query patterns, cluster auto-scaling controls, and pipeline execution efficiency. | Gain-sharing (% of verified 12-month cloud savings) | 20% – 30% of savings |
| **4. Managed DataOps & SLA Retainer** | Guaranteed pipeline uptime, data availability SLAs, automated schema drift detection, and rapid root-cause incident response. | Monthly Recurring Retainer | \$15,000 – \$35,000 / month |

---

## How We Calculate Pricing

Under outcome-based billing, pricing centers on **Pod Velocity** and **Fully Loaded Pod Sprint Costs**.

### 1. Fully Loaded Sprint Cost Formula
For a standard 5-person Delivery Pod over a 2-week sprint:

$$\text{Bi-Weekly Direct Pod Cost} = \sum (\text{Base Salaries} + \text{Taxes/Benefits}) + \text{Tooling Allocation}$$

* **Pod Composition:**
  - 1 Lead Data Engineer
  - 2 Senior Data Engineers
  - 1.5 Analytics Engineers
  - 0.5 DataOps / FinOps Engineer
* **Estimated Fully Loaded Pod Cost:** ~\$32,000 per 2-week sprint.

### 2. Pricing at Target Margin ($\ge 55\%$)
To hit a minimum project gross margin of 55%:

$$\text{Minimum Sprint Rate} = \frac{\text{Direct Pod Cost}}{1 - \text{Target Gross Margin}} = \frac{\$32,000}{1 - 0.55} = \mathbf{\$71,111 \text{ per sprint}}$$

### 3. Total Package Pricing Formula
When pricing fixed-outcome milestones:

$$\text{Outcome Price} = (\text{Estimated Sprints} \times \text{Base Sprint Rate}) + \text{Risk Buffer (10\% – 20\%)} + \text{Value Premium}$$

* **Example (3-Sprint Lakehouse Foundation):**
  - Base Pod Cost: $3 \times \$71,111 = \$213,333$
  - Add risk & value buffer $\approx \$235,000$ fixed fee.
  - If the pod delivers the DoD in 2.5 sprints using reusable template libraries, gross margin grows from 55% to $>62\%$.
