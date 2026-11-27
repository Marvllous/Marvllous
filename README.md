<h1 align="center">Marvellous Umeilechukwu</h1>

<p align="center">
  <strong>Data and Operations Analyst</strong><br>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/marvel7/">LinkedIn</a> ·
  <a href="mailto:marvellousug7@gmail.com">Email</a> ·
  London, UK
</p>

---

> I find what is broken in the data, quantify what it costs, and show teams how to fix it.

My background is operational, which shapes how I read data. I came up producing numbers that people acted on the same day, so I tend to skip past what a number is and go looking for why it moved, and then for what anyone is supposed to do about it. Banking, manufacturing, logistics, the question has been the same every time.

## 🔎 How I Work

I write the business question in plain English before I touch a query. What are we trying to find out, what data answers it, what does the answer look like. Then I validate every summary figure against a control total before I present it, because a clean looking dashboard built on an unverified join is worse than no dashboard.

I also try to be clear about where the evidence stops. In a sales and order review, nearly 20% of orders sat in a pending status. I could quantify the exposure and rule out the obvious causes, but the data could not tell me why. I said so, and left it flagged for investigation.

---

## 🛠 What I Can Do With Data

| Problem | How I handle it |
|---|---|
| **Data arrives split across systems** | Join multiple tables on shared keys so every record carries its full context, in SQL or Excel depending on scale |
| **One flat table cannot be analysed** | Model it into a fact table and dimensions, checking every key for conflicting attributes before collapsing it |
| **An assumption needs testing, not confirming** | Design the query so it can disprove the belief, then report what it actually shows |
| **The biggest bar is not the biggest problem** | Compare rates across groups instead of counts, so the largest group is not mistaken for the worst performing one |
| **Size is being mistaken for risk** | Separate exposure from failure rate, because the biggest balance and the biggest problem are often different things |
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
| **Power Query (M)** | Writing conditional columns that band continuous values, and that apply a calculation only to the records it should touch |
| **Calculated columns** | Bucketing continuous values into bands a business can act on, such as ageing in 30 day periods |
| **DAX date tables** | Building a continuous calendar so time based visuals do not break on gaps in the source |
| **M date tables** | Generating a parameter driven calendar that rebuilds itself when the data period changes |
| **Relationship management** | Diagnosing an inactive relationship that was silently flattening a chart, then repairing it |
| **Conditional formatting by measure** | Letting thresholds flag themselves as the data changes, instead of colouring by hand |
| **Decomposition trees** | Drilling exposure through product, segment, geography and branch type in one visual |

### Excel

| Capability | Applied to |
|---|---|
| **Excel Tables and XLOOKUP** | Joined tables on shared keys. Formulas name the column, not the cell, so they keep working when rows and columns are added |
| **Finding breaks that throw no error** | IDs with a space inside them. The lookup fails quietly, records drop out of every breakdown, and the headline total still looks right |
| **Pivot architecture** | Seven PivotTables on one shared cache, with slicers filtering the whole page from one click |
| **Picking the right average** | Banding categories against the median, not the mean, because one big value drags an average and puts the rest in the wrong group |

`SQL Server` `PostgreSQL` `Power BI` `Power Query` `DAX` `Excel`

---

## 🤝 How I Work With People

Most of my reporting gets read the same morning it goes out, and people act on it that day. You find out quickly when a number does not land, because someone comes back asking what it means. A report that needs explaining has already failed.

The question someone asks is rarely the whole question. Someone asking for last week's numbers usually has a decision sitting behind it, so I ask what they are deciding before I answer.

When the data can size a problem but not explain it, I say so. A guess that sounds right is worse than admitting you do not know, because people act on it.

---

## 💼 Experience

**Logistics Operations Associate, JD.com** · Jul 2025 to present

Run the daily operation of a last mile delivery station handling peaks above 600 parcels a day, from round allocation and dispatch for 8 to 10 drivers through to the daily, weekly and monthly reporting read each morning by station management, the regional head and other departments across the EU logistics network. The station holds a 99.6% fulfilment rate at Top 5 in the network and a 100% returns pickup rate at the No. 1 position.

Surface driver performance gaps early enough to act on them, by querying the station's retained delivery history in SQL to answer questions the standard reporting does not cover: how a named driver has performed month on month and year on year, pickups missed against pickups completed, and which customer complaints attach to them. The answer goes to my manager as a written report, or as an Excel or Power BI dashboard where it needs one.

Took daily round finish times from between 13:00 and 15:00 to around midday against a 15:00 cutoff on unchanged volume, by exporting the delivery manifest and rebuilding the allocation in pivot tables, clustering 200+ daily stops by recipient postcode and balancing round size against distance. The method is still how the station allocates.

Close 20 to 25 escalated exception cases a week on documented evidence instead of judgement, taking each case from both the driver on the round and the customer directly, and verifying the coordinates recorded on the proof of delivery against the customer's registered address and the door location in Google Maps to separate a genuine misdelivery from a false claim.

Moved the station to Top 10 across the EU network on customer experience, by working the complaint records as a dataset instead of a queue, isolating the recurring causes behind them and putting corrective actions against those causes, not against the individual cases.

Put the EU network's first third delivery wave into operation, building the case from the station's own volume and capacity data for a 19:00 round on top of the existing morning and afternoon waves, and tracking performance against that case once it was live.

**Data Analyst, Amdari** · Feb 2025 to present

Applied analytics programme, project delivery. Project work on industry datasets, each scoped to a business brief and delivered end to end. The projects below were delivered through this programme and through 10Alytics.

---

## 📁 Analytics Projects

Project based analytics on industry datasets, each scoped to a business brief and delivered end to end. Full documentation, queries, DAX, dashboards and raw source data are published in each repository, so every figure below can be reproduced from source.

| Project | Tools | Focus |
|---|---|---|
| [Bank Loan Default Analysis](https://github.com/Marvllous/bank-loan-default-analysis) | Power BI, Power Query, DAX | Loan defaults, arrears and loss concentration |
| [Loan Portfolio Risk Analysis](https://github.com/Marvllous/loan-portfolio-risk-analysis) | Power BI, DAX | Credit risk, defaults and exposure |
| [Production Downtime Analysis](https://github.com/Marvllous/production-downtime-analysis) | SQL Server, Power BI | Production downtime and bottlenecks |
| [Sales and Order Analysis](https://github.com/Marvllous/sales-and-order-analysis) | Excel | Sales, margin and channel analysis |

<br>

### [Bank Loan Default Analysis](https://github.com/Marvllous/bank-loan-default-analysis)
`Power BI` `Power Query` `DAX` · 2026

**Problem:** A bank holding 1,500 loans and $36.62M of lending could not tell in advance which loans would go bad. Its risk assessment was no longer keeping up, and the brief asked which borrower groups and loan types were driving the losses.

**What I did:** Built the transformation layer in Power Query, writing custom columns that band age, income, credit score and loan amount so continuous values could be grouped, and a conditional column that counts interest only on loans still being paid. Built a date table in M. Then worked out the default rate inside every band the bank records, instead of reading the tallest bar as the answer.

**What it showed:** Nothing the bank records predicts who defaults. The credit score bands do not order. Borrowers scoring 633 to 743 default on 20.5% of their lending, borrowers above 744 on 16.5%, and the 522 to 632 band defaults least of all at 13.1%. Loan size does not order either, with default rates sitting between 16% and 19% across every amount band. Of 1,500 loans, 925 paid off, 257 defaulted and 318 fell into arrears. The exposure that matters is not the $6.56M already written off. It is the $7.25M sitting in arrears, larger than everything lost to date and not yet counted as a loss.

<br>

### [Loan Portfolio Risk Analysis](https://github.com/Marvllous/loan-portfolio-risk-analysis)
`Power BI` `DAX` `Power Query` · 10Alytics, 2026

**Problem:** A lending dataset of 5,000 loans and $636.68M of lending, held in one flat table of 37 columns. No model behind it and no way to group, compare or drill into anything, so nobody could say where the credit risk sat.

**What I did:** Modelled it into a star schema with one fact table and six dimensions covering branch, calendar, collateral type, customer and loan type, testing every key for conflicting attributes before collapsing duplicates. Built a continuous calendar in DAX, held every measure in a dedicated table, and added a calculated column bucketing loan ageing into 30 day bands. Delivered a two page dashboard covering profit and loss, with cross-filtering, slicers and thresholds that flag themselves.

**What it showed:** 93.8% of the 209 defaults came from one customer segment holding 29% of the lending. Mortgage held 88% of the outstanding balance and under 10% of the failures, so the largest exposure and the real losses sat in different products. That moved the recommendation from collections to underwriting. Collections chases money that has already gone.

<br>

### [Production Downtime Analysis](https://github.com/Marvllous/production-downtime-analysis)
`SQL Server` `Power BI` · Amdari, 2025 to 2026

**Problem:** A manufacturing dataset covering 645 production batches at a site losing an estimated $1.5M a year to unplanned downtime, with no visibility on the cause. The brief recorded that management assumed operator error was the main driver.

**What I did:** Checked row counts and null distribution across all 13 factor columns before transforming anything, then used UNPIVOT to restructure those columns into rows that could be grouped and joined to the factor reference table. Measured each operator's delay rate as a share of their own batches using COUNT(DISTINCT) on both sides, because counting raw events would have penalised whoever ran the most work. Built a three page Power BI dashboard covering downtime factors, duration and operator scheduling, filtered by product, operator and date.

**What it showed:** 363 of 645 batches delayed, 21.74 days of production time lost. 610 of the 885 downtime events were non-operator, 68.93% by frequency and 70.14% by duration, so both measures land in the same place. Three of the top four causes were process and supply: cleaning and sanitation cycles, raw material shortage and scheduling delays. The fix moved away from performance management and towards maintenance scheduling, supply and cleaning cycle planning.

<br>

### [Sales and Order Analysis](https://github.com/Marvllous/sales-and-order-analysis)
`Excel` · Amdari, 2026

**Problem:** One month of sales and order data for a beverage distributor, held in three unlinked tables carrying 259 rows for 250 real orders, inconsistent text fields and dates stored as serial numbers. Revenue was visible, what drove it was not.

**What I did:** Reconciled the order table to 250 unique orders, standardised a status field that appeared in 15 spellings, joined all three tables on ID so every line carries the customer's county, type and preferred channel alongside the product's category, size and cost, then built gross sales, cost, discount and profit at line level. Validated every total against a control figure.

**What it showed:** 250 orders, €12,960.50 gross, 44.4% margin. Customers who order by phone account for €4,773.30, or 36.8% of revenue, twice the next channel and more than online and sales reps put together, which sits awkwardly against any plan to push harder into digital. Water leads the categories on revenue and sits near the bottom on profit per unit, while energy drinks, the smallest category at 11.3%, hold the highest margin product of all twenty.

---

## 🎓 Background

**MSc Project Management**, Ravensbourne University, London

**LLB Law**, Igbinedion University, Nigeria

**Professional Development**

**10Alytics** · 2026 to present

Applied analytics programme. Instructor-led curriculum covering Excel, Power BI and Power BI Service, SQL, Tableau, Microsoft Fabric, Python and AI-assisted analytics.

**Certifications**
- Google Data Analytics Professional Certificate
- Supply Chain Logistics, Rutgers University via Coursera

---

## 📬 Contact

**Email:** marvellousug7@gmail.com

**LinkedIn:** [linkedin.com/in/marvel7](https://www.linkedin.com/in/marvel7/)

**CV:** [View my CV](Marvellous-Umeilechukwu-CV.pdf)
