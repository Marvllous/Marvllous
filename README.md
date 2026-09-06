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

Three examples of what that means in practice:

- Unpivoted 13 downtime factor columns into rows across 645 production batches to isolate what was actually causing delays. Result: 69% of downtime was systemic, not operator error, which moved the fix from performance management to maintenance scheduling.
- Joined three unlinked tables on ID and rebuilt profit at line level, which showed the largest revenue category was one of the thinnest on margin while the smallest category held the highest-margin product in the range.
- Built a weighted engagement score across 9 genres and 999 users, combining completion rate, repeat viewing and churn risk, to rank where content spend was returning and where it was not.

---

## 🛠 Tools and Techniques

![SQL](https://img.shields.io/badge/SQL-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)
![Excel](https://img.shields.io/badge/Excel-217346?style=flat-square&logo=microsoftexcel&logoColor=white)

| Technique | Where I have used it |
|---|---|
| **CTEs** | Comparing scheduled against actual start times to surface data discrepancies before analysis |
| **UNPIVOT** | Converting 13 wide downtime factor columns into a queryable row structure |
| **DATEDIFF** | Calculating actual batch duration against planned duration to quantify delay |
| **CASE logic** | Splitting downtime events into operator and non operator error for root cause attribution |
| **Multi-table joins** | Linking products, batches, downtime events and factor definitions across four tables |
| **Power Query and DAX** | Cleaning source data and building measures behind a three page Power BI dashboard |
| **Excel lookups and pivots** | Merging customer, product and order tables on ID, then aggregating to category and channel level |
| **Weighted scoring models** | Combining multiple engagement metrics into a single comparable genre ranking |
| **Control total validation** | Checking every summary figure against a known total before publishing it |

---

## 📁 Projects

| Project | Tools | Focus |
|---|---|---|
| [Emerald Springs Bottling](https://github.com/Marvllous/emerald-springs-sales-analysis) | Excel | Sales, margin and channel analysis |
| GreenTech Manufacturing | SQL Server, Power BI | Production downtime and bottlenecks |
| StreamWave Entertainment | Excel | Viewer engagement and content ROI |

<br>

### [Emerald Springs Bottling, Sales and Order Analysis](https://github.com/Marvllous/emerald-springs-sales-analysis)
`Excel`

**Problem:** A beverage distributor could see revenue but not what was driving it. Three unlinked tables, inconsistent text fields, dates stored as serial numbers.

**What I did:** Standardised text with TRIM, CLEAN and PROPER, converted serial dates, joined all three tables on Customer_ID and Product_ID, then built gross sales, cost, discount and profit at line level. Validated every total against a control figure.

**What it showed:** 250 orders, €12,960.50 gross, 44.4% margin. One channel out-earned two others combined. The largest revenue category ranked near the bottom on profit per unit, while the smallest category contained the highest-margin product of all 20 in the range.

<br>

### GreenTech Manufacturing, Production Downtime Analysis
`SQL Server` `Power BI` · *repository in progress*

**Problem:** An eco-products manufacturer losing an estimated $1.5M a year to unplanned downtime, with no visibility on the cause.

**What I did:** Queried four tables in SQL Server. Used UNPIVOT to restructure 13 factor columns into rows, DATEDIFF to calculate actual against planned duration, CTEs to validate timestamp discrepancies, and CASE logic to separate operator from systemic causes. Built a three page Power BI dashboard covering downtime factors, duration analysis and operator scheduling.

**What it showed:** 645 batches analysed, 56% delayed, 21.74 days of production time lost. 69% of downtime was systemic rather than human error. Cleaning and sanitation was the single largest cause at 86 occurrences, followed by raw material shortage at 77.

<br>

### StreamWave Entertainment, Viewer Engagement Analysis
`Excel` · *repository in progress*

**Problem:** A streaming platform spreading content investment across genres without data behind the decision.

**What I did:** Imported four raw CSV files across seven sheets. Merged user and content data with VLOOKUP, calculated completion rate, repeat viewing and churn risk with statistical functions, then built a weighted scoring model to rank all 9 genres on a single scale. Delivered an interactive dashboard with genre and time slicers.

**What it showed:** 999 users analysed. Drama and Comedy led every metric. Biography and Musical together accounted for under 0.2% of engagement while still absorbing budget. New subscriptions peaked June to July then declined, with cancellations rising over the same window.

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
