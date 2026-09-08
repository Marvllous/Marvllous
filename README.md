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

My background is operational, so I approach analysis the way an operations team would: start with the metric, find the gap, work out what is driving it, then say what should change. My project work has covered a range of business problems, from sales and margin analysis to production efficiency and customer engagement. If the analysis does not lead to a decision, it is not finished.

---

## 🔎 How I Work

Most analysis fails for one of two reasons. Either the question was never defined properly, or the answer never reached anyone who could act on it.

I write the business question in plain English before I touch a query. What are we trying to find out, what data answers it, what does the answer look like. Then I validate every summary figure against a control total before I present it, because a clean looking dashboard built on an unverified join is worse than no dashboard.

I also try to be clear about where the evidence stops. On my last project I found nearly 20% of orders sitting in a pending status. I could quantify the exposure and rule out the obvious causes, but the data could not tell me why. I said so, rather than inventing a reason that sounded better.

---

## 🛠 What I Can Do With Data

| Problem | How I handle it |
|---|---|
| **Data arrives split across systems** | Join multiple tables on shared keys so every record carries its full context, in SQL or Excel depending on scale |
| **Raw data is not analysis ready** | Validate the source before transforming it, then restructure wide tables into a queryable shape and correct data types |
| **Nobody knows what is driving a number** | Break the metric down across dimensions until the driver isolates, then quantify what it costs |
| **An assumption needs testing, not confirming** | Design the query so it can disprove the belief, then report what it actually shows |
| **A comparison is not like for like** | Build rates rather than raw counts, so volume differences do not distort the ranking |
| **A metric needs to be built, not just read** | Construct calculated measures at row level, including margin, duration variance and weighted scoring models |
| **Stakeholders cannot read a spreadsheet** | Build interactive dashboards with filtering, so the same report answers several people's questions |
| **The numbers need to be trusted** | Validate every figure against a control total before it goes anywhere |

### SQL

| Capability | Applied to |
|---|---|
| **Views** | Encapsulating transformation logic so downstream queries stay clean and reusable |
| **UNPIVOT** | Reshaping wide tables into row structures that can be aggregated and joined |
| **CTEs** | Staging validation checks before analysis runs |
| **CASE logic** | Conditional attribution, splitting causes into categories for root cause analysis |
| **COUNT(DISTINCT)** | Building comparable rates across groups of unequal size |
| **DATEDIFF** | Calculating duration variance against planned targets |
| **Multi-table joins** | Linking four related tables through fact and dimension keys |

`SQL Server` `PostgreSQL` `Power BI` `Power Query` `DAX` `Excel`

---

## 📁 Projects

| Project | Tools | Focus |
|---|---|---|
| [Emerald Springs Bottling](https://github.com/Marvllous/emerald-springs-sales-analysis) | Excel | Sales, margin and channel analysis |
| [GreenTech Manufacturing](https://github.com/Marvllous/greentech-production-downtime-analysis) | SQL Server, Power BI | Production downtime and bottlenecks |
| StreamWave Entertainment | Excel | Viewer engagement and content ROI |

<br>

### [Emerald Springs Bottling, Sales and Order Analysis](https://github.com/Marvllous/emerald-springs-sales-analysis)
`Excel`

**Problem:** A beverage distributor could see revenue but not what was driving it. Three unlinked tables, inconsistent text fields, dates stored as serial numbers.

**What I did:** Cleaned and standardised the source data, joined all three tables on ID, then built gross sales, cost, discount and profit at line level. Validated every total against a control figure.

**What it showed:** 250 orders, €12,960.50 gross, 44.4% margin. One channel out-earned two others combined. The largest revenue category ranked near the bottom on profit per unit, while the smallest category held the highest margin product of all 20 in the range.

<br>

### [GreenTech Manufacturing, Production Downtime Analysis](https://github.com/Marvllous/greentech-production-downtime-analysis)
`SQL Server` `Power BI`

**Problem:** A manufacturer losing an estimated $1.5M a year to unplanned downtime, with no visibility on the cause. Management assumed operator error was the main driver.

**What I did:** Validated the source data before transforming it, then used UNPIVOT to restructure 13 downtime factor columns into a queryable format. Tested the operator-error assumption directly against the factor reference table rather than accepting it. Built a three page Power BI dashboard covering downtime factors, duration and operator scheduling.

**What it showed:** 645 batches, 56% delayed, 21.74 days of production time lost. 69% of downtime was systemic rather than operator error, which moved the fix away from performance management and towards maintenance scheduling and material supply.

<br>

### StreamWave Entertainment, Viewer Engagement Analysis
`Excel` · *repository in progress*

**Problem:** A streaming platform investing across genres without data behind the decision.

**What I did:** Merged four raw datasets, calculated completion rate, repeat viewing and churn risk, then built a weighted scoring model to rank all 9 genres on a single comparable scale. Delivered an interactive dashboard with genre and time filtering.

**What it showed:** 999 users analysed. Drama and Comedy led every metric. Two genres accounted for under 0.2% of engagement between them while still absorbing budget. Subscriptions peaked June to July then declined as cancellations rose.

---

## 💼 Experience

**Data Analytics Consultant, Amdari**

Project based analytics across multiple business contexts. Analysed large datasets, built interactive dashboards tracking KPIs including downtime rate, completion rate and engagement metrics, and delivered recommendations that supported process improvements. The projects above came from this work.

<br>

**Logistics Operations Coordinator, JD.com**

Daily operational reporting for a delivery station covering fulfilment rate, pickup rate, route efficiency and complaint data. The station holds a 99.6% fulfilment rate, top five in Europe, and a 100% pickup rate ranking first EU wide.

Ran root cause analysis on customer complaint data and used the findings to drive corrective actions, moving the station into the top ten across the EU on that measure. Benchmarked performance across 50+ daily delivery stops to identify route efficiency gaps.

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
