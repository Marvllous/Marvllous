<h1 align="center">Marvellous Umeilechukwu</h1>

<p align="center">
  <strong>Data Analyst</strong><br>
  SQL · Power BI · Excel
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/marvel7/">LinkedIn</a> ·
  <a href="mailto:marvellousug7@gmail.com">Email</a> ·
  London, UK
</p>

---

> I find what is broken in the data, quantify what it costs, and show teams how to fix it.

My background is operational, which shapes how I read a dataset. I am less interested in what a number is than in why it moved, and less interested in why it moved than in what someone should do about it. The domain changes, the question does not.

## 🔎 How I Work

I write the business question in plain English before I touch a query. What are we trying to find out, what data answers it, what does the answer look like. Then I validate every summary figure against a control total before I present it, because a clean looking dashboard built on an unverified join is worse than no dashboard.

I also try to be clear about where the evidence stops. On my last project I found nearly 20% of orders sitting in a pending status. I could quantify the exposure and rule out the obvious causes, but the data could not tell me why. I said so, rather than inventing a reason that sounded better.

I use Claude and ChatGPT for the parts of the job where a second opinion is faster than working alone. Getting DAX syntax right, diagnosing why a visual is not behaving, and stress testing my reasoning before I commit to a conclusion. On the Horizon Trust build one chart was silently flattening every bar, and talking through the model rather than the data is what surfaced an inactive relationship behind it. What I do not do is hand over client data. The tools help with method and logic. The data stays where it belongs.

---

## 🛠 What I Can Do With Data

| Problem | How I handle it |
|---|---|
| **Data arrives split across systems** | Join multiple tables on shared keys so every record carries its full context, in SQL or Excel depending on scale |
| **Raw data is not analysis ready** | Validate the source before transforming it, then restructure wide tables into rows that can be grouped and joined, and correct the data types |
| **One flat table cannot be analysed** | Model it into a fact table and dimensions, checking every key for conflicting attributes before collapsing it |
| **Nobody knows what is driving a number** | Break the metric down across dimensions until I can isolate what is driving it, then quantify what it costs |
| **An assumption needs testing, not confirming** | Design the query so it can disprove the belief, then report what it actually shows |
| **A comparison is not like for like** | Build rates rather than raw counts, so volume differences do not distort the ranking |
| **A metric needs to be built, not just read** | Construct calculated measures at row level, including margin, cost and duration variance against plan |
| **Size is being mistaken for risk** | Separate exposure from failure rate, because the biggest balance and the biggest problem are often different things |
| **Stakeholders cannot read a spreadsheet** | Build interactive dashboards with filtering, so the same report answers several people's questions |
| **The numbers need to be trusted** | Validate every figure against a control total before it goes anywhere |

### SQL

| Capability | Applied to |
|---|---|
| **Views** | Holding transformation logic in one place so downstream queries stay clean and reusable |
| **UNPIVOT** | Reshaping wide tables into rows that can be grouped and joined |
| **CTEs** | Staging validation checks before analysis runs |
| **CASE logic** | Splitting causes into categories so root causes can be attributed properly |
| **COUNT(DISTINCT)** | Building comparable rates across groups of unequal size |
| **DATEDIFF** | Calculating duration variance against planned targets |
| **Multi-table joins** | Linking four related tables through fact and dimension keys |

### Power BI

| Capability | Applied to |
|---|---|
| **Star schema modelling** | Splitting one flat table of 37 columns into a fact table and six dimensions so measures aggregate correctly |
| **Key integrity validation** | Testing every dimension key for conflicting attributes before removing duplicates, so nothing is lost silently |
| **DAX measures** | Building rates, distinct counts and filtered aggregates that respond to every slicer on the page |
| **Calculated columns** | Bucketing continuous values into bands a business can act on, such as ageing in 30 day periods |
| **DAX date tables** | Building a continuous calendar so time based visuals do not break on gaps in the source |
| **Relationship management** | Diagnosing an inactive relationship that was silently flattening a chart, then repairing it |
| **Conditional formatting by measure** | Letting thresholds flag themselves as the data changes, rather than colouring by hand |
| **Decomposition trees** | Drilling exposure through product, segment, geography and branch type in one visual |

`SQL Server` `PostgreSQL` `Power BI` `Power Query` `DAX` `Excel` `Claude` `ChatGPT`

---

## 🤝 How I Work With People

Analysis only counts once someone acts on it, so most of the job is communication.

I write for the person reading, not for the analyst who built it. That means leading with the decision rather than the method, giving stakeholders a dashboard they can filter themselves instead of a static report they have to ask me about, and being direct about what a number does not tell you.

Two habits from outside analytics carry the most weight. Project Management taught me to work backwards from the outcome someone needs. Law taught me to build an argument from evidence and expect it to be challenged, which is a useful instinct when your conclusion contradicts what a team already believes.

---

## 📁 Projects

| Project | Tools | Focus |
|---|---|---|
| [Horizon Trust Bank](https://github.com/Marvllous/horizon-trust-loan-portfolio-risk-analysis) | Power BI, DAX | Credit risk, defaults and exposure |
| [GreenTech Manufacturing](https://github.com/Marvllous/greentech-production-downtime-analysis) | SQL Server, Power BI | Production downtime and bottlenecks |
| [Emerald Springs Bottling](https://github.com/Marvllous/emerald-springs-sales-analysis) | Excel | Sales, margin and channel analysis |

<br>

### [Horizon Trust Bank, Loan Portfolio Risk Analysis](https://github.com/Marvllous/horizon-trust-loan-portfolio-risk-analysis)
`Power BI` `DAX` `Power Query`

**Problem:** A commercial bank with $636.68M lent across 5,000 loans could not see where its credit risk sat. Everything lived in one flat table of 37 columns, with no model behind it and no way to group, compare or drill into anything.

**What I did:** Modelled it into a star schema with a fact table and six dimensions, testing every key for conflicting attributes before collapsing duplicates. Built a continuous calendar in DAX, held every measure in a dedicated table, and added a calculated column bucketing loan ageing into 30 day bands. Delivered a two page dashboard covering profit and loss, with cross-filtering, slicers and thresholds that flag themselves.

**What it showed:** 93.8% of the bank's 209 defaults came from one customer segment holding 29% of the lending. Mortgage held 88% of the outstanding balance and under 10% of the failures, so the largest exposure and the actual losses sat in different products entirely. Branch lending volume varied 1.4 times across 20 branches while default rate varied 2.8 times, which moved the question away from lending scale and towards how credit decisions are made locally.

<br>

### [GreenTech Manufacturing, Production Downtime Analysis](https://github.com/Marvllous/greentech-production-downtime-analysis)
`SQL Server` `Power BI`

**Problem:** A manufacturer losing an estimated $1.5M a year to unplanned downtime, with no visibility on the cause. Management assumed operator error was the main driver.

**What I did:** Validated the source data before transforming it, then used UNPIVOT to restructure 13 downtime factor columns into rows that could be grouped and joined. Tested the operator-error assumption directly against the factor reference table rather than accepting it. Built a three page Power BI dashboard covering downtime factors, duration and operator scheduling.

**What it showed:** 645 batches, 56% delayed, 21.74 days of production time lost. 69% of 885 downtime events came from process and supply failures rather than operator error, which moved the fix away from performance management and towards maintenance scheduling and material supply.

<br>

### [Emerald Springs Bottling, Sales and Order Analysis](https://github.com/Marvllous/emerald-springs-sales-analysis)
`Excel`

**Problem:** A beverage distributor could see revenue but not what was driving it. Three unlinked tables, inconsistent text fields, dates stored as serial numbers.

**What I did:** Cleaned and standardised the source data, joined all three tables on ID, then built gross sales, cost, discount and profit at line level. Validated every total against a control figure.

**What it showed:** 250 orders, €12,960.50 gross, 44.4% margin. One channel out-earned two others combined. The largest revenue category ranked near the bottom on profit per unit, while the smallest category held the highest margin product of all 20 in the range.

---

## 💼 Experience

**Data Analytics Consultant, 10Alytics** · Jul 2026 to present

Project based analytics on commercial and financial data. Cleaned and connected disconnected source tables, rebuilt profit at line level, and delivered margin and channel analysis with an interactive Excel dashboard. Modelled a 5,000 record loan portfolio into a star schema and built a two page Power BI credit risk dashboard covering lending performance, default concentration and exposure. The Emerald Springs and Horizon Trust analyses above came from this work.

<br>

**Logistics Operations Associate, JD.com** · Jul 2025 to present

I build and maintain the daily operational reporting for a delivery station, covering fulfilment rate, pickup rate, route efficiency and complaint data. The station reached a 99.6% fulfilment rate, ranking Top 5 in Europe, and a 100% pickup rate that took the No. 1 position EU-wide.

Analyse 200+ daily delivery stops in Excel using pivot tables to break performance down by route and by driver. Ran root cause analysis on customer complaint data and used the findings to drive corrective actions, ranking the station Top 10 across the EU on that measure.

<br>

**Data Analytics Consultant, Amdari** · Feb 2025 to Jun 2026

Project based analytics across production and media data. Restructured raw operational data for analysis, built dashboards tracking KPIs including downtime rate and production efficiency, and delivered recommendations that supported process improvements. The GreenTech analysis above came from this work.

---

## 🎓 Background

**MSc Project Management**, Ravensbourne University, London
**LLB Law**, Igbinedion University, Nigeria

**Certifications**
- IBM Data Analyst Professional Certificate
- Google Data Analytics Professional Certificate
- Supply Chain Logistics, Rutgers University via Coursera

---

## 📬 Contact

**Email:** marvellousug7@gmail.com

**LinkedIn:** [linkedin.com/in/marvel7](https://www.linkedin.com/in/marvel7/)

**CV:** [View my CV](Marvellous-Umeilechukwu-CV.pdf)
