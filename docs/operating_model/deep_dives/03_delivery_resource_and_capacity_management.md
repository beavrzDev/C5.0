# Deep Dive: Delivery, Resource & Capacity Management (Function 03)

## Why Delivery and Resourcing Are One Function
At 20 people, Technical Delivery and Resource Management run as a single unit to prevent gaps between deal closing, project execution, and engineer staffing. The **Data Delivery Manager** and **Principal Data Architects** share responsibility for assigning engineers to projects, matching skills to work, maintaining delivery quality, and hitting utilization targets.

---

## Leadership Structure & Time Allocation

```
                       +-----------------------------------+
                       |    Principal Data Architects (2)  |
                       |  (Strategy, Presales & Quality QA)|
                       +-----------------+-----------------+
                                         |
                                         v
                       +-----------------------------------+
                       |    Data Delivery Manager (1)      |
                       |    (Staffing & Scheduling)        |
                       +-----------------+-----------------+
                                         |
            +----------------------------+----------------------------+
            |                            |                            |
            v                            v                            v
  +-------------------+        +-------------------+        +-------------------+
  |   Delivery Pod 1  |        |   Delivery Pod 2  |        |   Delivery Pod 3  |
  |  (5 people/client)|        |  (5 people/client)|        |  (5 people/client)|
  +-------------------+        +-------------------+        +-------------------+
```

### Leadership Responsibilities & Utilization Targets

| Role | Delivery & Execution | Staffing & Capacity | Presales & Architecture QA | Target Utilization |
| :--- | :--- | :--- | :--- | :--- |
| **Principal Data Architects (2)** | Architecture reviews & escalation support | Skill inventory and technical matching | Scoping SOWs, architecture audits, partner technical alignment | 30% – 40% |
| **Data Delivery Manager (1)** | Agile sprint cadence, scope change controls, milestone delivery | Weekly assignment scheduling, bench management, time tracking | Capacity forecasting against CRM deal pipeline | 0% (Internal Overhead) |
| **Lead Data Engineers (3)** | Hands-on code leadership, daily standups, pull request (PR) approvals | Pod-level workload distribution, mentoring junior/mid engineers | Technical scoping validation | 70% – 80% |

---

## Pod Staffing & Skill-Based Assignment

Engineers are assigned in standardized, cross-functional **Delivery Pods** specialized on **Databricks** and cloud architectures — not allocated one-by-one.

```
  +-----------------------------------------------------------------------+
  |                        STANDARD DELIVERY POD                          |
  |                                                                       |
  |  +--------------------+  +--------------------+  +-----------------+  |
  |  |  Lead Data Eng (1) |  | Senior Data Eng (2)|  | Analytics Eng   |  |
  |  |  (Tech & Client)   |  | (Ingestion/Spark)  |  | (1.5) (Models)  |  |
  |  +--------------------+  +--------------------+  +-----------------+  |
  |                                                                       |
  |             +-------------------------------------------+             |
  |             | DataOps / FinOps Specialist (0.5)         |             |
  |             | (IaC, CI/CD, Observability & Cost Audits) |             |
  |             +-------------------------------------------+             |
  +-----------------------------------------------------------------------+
```

### Standard Pod Composition (5 people)
* **1 Lead Data Engineer:** Technical architect on the ground, client technical counterpart, PR reviewer.
* **2 Senior Data Engineers:** Core pipeline engineering, streaming/batch ingestion connectors, Spark & Databricks lakehouse structuring.
* **1.5 Analytics Engineers:** Data transformation modeling, semantic layer build-out, lakehouse BI dataset optimization.
* **0.5 DataOps / FinOps Engineer:** CI/CD runners, Infrastructure-as-Code (Terraform), cloud compute monitoring & cluster optimization.

---

## Skill Matrix & Keeping People Assigned

Data engineers can't simply be swapped between different technology stacks. To keep people productively assigned, allocation is tracked against a live **Skill Inventory Matrix**:

* **Primary Stack:** Databricks (Lakehouse, Unity Catalog, Delta Live Tables, Spark), Cloud Partners (AWS, Azure, GCP), SQL / Transformation Modeling, and Infrastructure-as-Code (Terraform).
* **Capacity Buffer Rule:** No engineer is booked beyond **90% billable capacity** — the 10% reserve goes to practice R&D, peer PR reviews, and internal IP development.
* **Shadowing Protocol:** When expanding junior or mid-level engineers into advanced platform capabilities, **0.25** of an engineer's time is assigned to shadow a Senior Lead to cross-train without billing the client.

---

## How a Project Moves Through the Firm

```
[ CRM Deal Pipeline ] (Stage 3: Proposal)
         │
         ▼
 ┌─────────────────────────────────────────────────────────┐
 │ STEP 1: Capacity & Skill Match Check                    │
 │ • Data Delivery Manager checks 6-week resource forecast  │
 │ • Principal Architect tags required stack skills        │
 └─────────────────────────┬───────────────────────────────┘
                           │
                           ▼
 ┌─────────────────────────────────────────────────────────┐
 │ STEP 2: Pod Setup & Kickoff                             │
 │ • Assign Pod Lead & lock team in scheduling tool        │
 │ • Deploy standard IaC & lakehouse codebase templates    │
 └─────────────────────────┬───────────────────────────────┘
                           │
                           ▼
 ┌─────────────────────────────────────────────────────────┐
 │ STEP 3: Sprint Execution & Quality Checks               │
 │ • 2-week sprint cycles with automated data tests        │
 │ • Weekly Principal Architect code & architecture review │
 └─────────────────────────┬───────────────────────────────┘
                           │
                           ▼
 ┌─────────────────────────────────────────────────────────┐
 │ STEP 4: Project Close & Asset Capture                   │
 │ • Transition to Managed DataOps or hand off to client   │
 │ • Move reusable pipeline macros & IaC into IP library   │
 └─────────────────────────┬───────────────────────────────┘
```

### Step Details

#### Step 1: Sales-to-Resourcing Intake (3 Weeks Before Kickoff)
* Deals reaching **70%+ win probability** in the CRM automatically trigger a provisional hold in the scheduling system.
* The Data Delivery Manager and Principal Architect review stack requirements and confirm pod lead availability.

#### Step 2: Pod Setup & Kickoff
* The team assignment is formally locked in the Professional Services Automation (PSA) platform.
* Standard project templates (IaC repositories, pre-configured transformation templates, CI/CD linters) are cloned and tailored to the client.

#### Step 3: Sprint Execution & Quality Checks
* Delivery runs on **2-week sprints**.
* Every sprint ends with automated data test validation (schema checks, freshness checks, regression tests).
* Weekly Principal Architect sign-offs ensure compliance with enterprise standards.

#### Step 4: Project Close & Asset Capture
* At milestone completion, client projects move to either a monthly **Managed DataOps Retainer** or are handed off to client internal staff.
* Reusable macros, transformation queries, and IaC modules are reviewed and added to the **Practice Dev & IP Lab**.
* Engineers coming off projects (3+ business days unassigned) automatically move to IP development tasks.

---

## Key Metrics

| Metric | Target (20 People) | Measured | Primary Owner | When to Escalate |
| :--- | :--- | :--- | :--- | :--- |
| **Team Billable Utilization** | $\ge 75\%$ average | Weekly | Data Delivery Manager | Utilization below $70\%$ for 2 consecutive weeks |
| **Project Gross Margin** | $> 50\%$ (Target $\ge 55\%$) | Monthly per SOW | Principal Data Architects | Margin below $45\%$ due to scope creep |
| **On-Time Milestone Delivery** | $\ge 90\%$ | Bi-weekly | Data Delivery Manager | Sprint deliverables delayed by $>3$ business days |
| **Bench Rate** | $< 8\%$ of total billable hours | Weekly | Data Delivery Manager | Unassigned time exceeds $10\%$ of total capacity |
| **Peer Review Coverage** | $100\%$ of merged PRs | Continuous | Lead Data Engineers | Code deployed to production without architectural sign-off |

---

## Software Stack (By Category)
* **PSA & Resource Management:** Resource scheduling & capacity planning platform (integrated with CRM deal stages).
* **Sprint & Task Management:** Agile issue tracker (pre-configured data engineering workflow templates).
* **Time & Milestone Tracking:** Project time & milestone tracking platform (linked to SOW milestone deliverables, not individual timesheets).
* **Technical Infrastructure & CI/CD:** Enterprise Git repository, automated CI/CD runners, Infrastructure-as-Code tooling, and data observability / automated testing suites.

---

## Growth Triggers (20 → 60 → 100 People)
* **At 35 People:** Split the combined role. The Data Delivery Manager focuses exclusively on project execution. A dedicated **Resource Operations Lead** handles complex scheduling across 6+ simultaneous client pods.
* **At 60 People:** Decentralize into specialized practice domains (Lakehouse Architecture, Real-Time Streaming, FinOps/Governance, and MLOps/AI). Add nearshore delivery pods (LatAm / Eastern Europe) managed by US Lead Architects to protect margins.
* **At 100 People:** Upgrade to an enterprise PSA platform with automated skill-matching and real-time revenue recognition. Stand up a 24/7 global Resource Operations Center to support managed DataOps services.
