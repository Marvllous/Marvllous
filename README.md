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

I also try to be clear about where the evidence stops. In a sales and order review, nearly 20% of orders sat in a pending status. I could quantify the exposure and rule out the obvious causes, but the data could not tell me why. I said so, instead of inventing a reason that sounded better.

---

## 🛠 What I Can Do With Data

| Problem | How I handle it |
|---|---|
| **Data arrives split across systems** | Join multiple tables on shared keys so every record carries its full context, in SQL or Excel depending on scale |
| **Raw data is not analysis ready** | Validate the source before transforming it, then restructure wide tables into rows that can be grouped and joined, and correct the data types |
| **One flat table cannot be analysed** | Model it into a fact table and dimensions, checking every key for conflicting attributes before collapsing it |
| **Nobody knows what is driving a number** | Break the metric down across dimensions until I can isolate what is driving it, then quantify what it costs |
| **An assumption needs testing, not confirming** | Design the query so it can disprove the belief, then report what it actually shows |
| **The biggest bar is not the biggest problem** | Compare rates across groups instead of counts, so the largest group does not get mistaken for the worst performing one |
| **A comparison is not like for like** | Build rates instead of raw counts, so volume differences do not distort the ranking |
| **A metric needs building, not reading** | Construct calculated measures at row level, including margin, cost and duration variance against plan |
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

`SQL Server` `PostgreSQL` `Power BI` `Power Query` `DAX` `Excel` `Claude`

---

## 🤝 How I Work With People

Most of my reporting gets read the same morning it goes out, and people act on it that day. You find out quickly when a number does not land, because someone comes back asking what it means. A report that needs explaining has already failed.

The question someone asks is rarely the whole question. Someone asking for last week's numbers usually has a decision sitting behind it, so I ask what they are deciding before I answer.

When the data can size a problem but not explain it, I say so. A guess that sounds right is worse than admitting you do not know, because people act on it.

---

## 📁 Analytics Projects

Project based analytics on industry datasets, each scoped to a business brief and delivered end to end. Full documentation, queries, DAX, dashboards and raw source data are published in each repository, so every figure below can be reproduced instead of taken on trust.

| Project | Tools | Focus |
|---|---|---|
| [Bank Loan Default Analysis](https://github.com/Marvllous/bank-loan-default-analysis) | Power BI, Power Query, DAX | Loan defaults, arrears and loss concentration |
| [Loan Portfolio Risk Analysis](https://github.com/Marvllous/loan-portfolio-risk-analysis) | Power BI, DAX | Credit risk, defaults and exposure |
| [Production Downtime Analysis](https://github.com/Marvllous/production-downtime-analysis) | SQL Server, Power BI | Production downtime and bottlenecks |
| [Sales and Order Analysis](https://github.com/Marvllous/sales-and-order-analysis) | Excel | Sales, margin and channel analysis |

<br>

### [Bank Loan Default Analysis](https://github.com/Marvllous/bank-loan-default-analysis)
`Power BI` `Power Query` `DAX` · Amdari, 2026

**Problem:** A bank holding 1,500 loans and $36.62M of lending could not tell in advance which loans would go bad. Its risk assessment was no longer keeping up, and the brief asked which borrower groups and loan types were driving the losses.

**What I did:** Built the transformation layer in Power Query, banding age, income, credit score and loan amount so continuous values could be grouped, and writing a conditional column that counts interest only on loans still being paid. Built a date table in M. Then worked out the default rate for every borrower group the bank records, instead of reading the tallest bar as the answer.

**What it showed:** None of the characteristics the bank collects separate defaulters from repayers. Employed borrowers default at 16.88% and unemployed at 17.87%, and the credit score bands do not rise or fall in order, so the score is not tracking anything. The bank also charges roughly 6% across every score band, so it is not pricing for risk either. The loss concentrates by size instead. Loans above $44k are 17.3% of the book and 40.1% of the $6.56M lost. A further $7.25M sits in arrears, more than has already been written off.

<br>

### [Loan Portfolio Risk Analysis](https://github.com/Marvllous/loan-portfolio-risk-analysis)
`Power BI` `DAX` `Power Query` · Amdari, 2026

**Problem:** A lending dataset of 5,000 loans and $636.68M of lending, held in one flat table of 37 columns. No model behind it and no way to group, compare or drill into anything, so nobody could say where the credit risk sat.

**What I did:** Modelled it into a star schema with a fact table and six dimensions, testing every key for conflicting attributes before collapsing duplicates. Built a continuous calendar in DAX, held every measure in a dedicated table, and added a calculated column bucketing loan ageing into 30 day bands. Delivered a two page dashboard covering profit and loss, with cross-filtering, slicers and thresholds that flag themselves.

**What it showed:** 93.8% of the 209 defaults came from one customer segment holding 29% of the lending. Mortgage held 88% of the outstanding balance and under 10% of the failures, so the largest exposure and the actual losses sat in different products entirely. Branch lending volume varied 1.4 times across 20 branches while default rate varied 2.8 times, which moved the question away from lending scale and towards how credit decisions are made locally.

<br>

### [Production Downtime Analysis](https://github.com/Marvllous/production-downtime-analysis)
`SQL Server` `Power BI` · Amdari, 2025 to 2026

**Problem:** A manufacturing dataset covering 645 production batches at a site losing an estimated $1.5M a year to unplanned downtime, with no visibility on the cause. The brief recorded that management assumed operator error was the main driver.

**What I did:** Validated the source data before transforming it, then used UNPIVOT to restructure 13 downtime factor columns into rows that could be grouped and joined. Tested the operator-error assumption directly against the factor reference table instead of accepting it. Built a three page Power BI dashboard covering downtime factors, duration and operator scheduling.

**What it showed:** 645 batches, 56% delayed, 21.74 days of production time lost. 69% of 885 downtime events were non-operator, which moved the fix away from performance management and towards maintenance scheduling, supply and cleaning cycle planning.

<br>

### [Sales and Order Analysis](https://github.com/Marvllous/sales-and-order-analysis)
`Excel` · Amdari, 2026

**Problem:** One month of sales and order data for a beverage distributor, held in three unlinked tables carrying 259 rows for 250 real orders, inconsistent text fields and dates stored as serial numbers. Revenue was visible, what drove it was not.

**What I did:** Reconciled the order table to 250 unique orders, standardised a status field that appeared in 15 spellings, joined all three tables on ID, then built gross sales, cost, discount and profit at line level. Validated every total against a control figure.

**What it showed:** 250 orders, €12,960.50 gross, 44.4% margin. One third of revenue sits with customers who prefer a single ordering channel. The largest revenue category ranked near the bottom on profit per unit, while the smallest category held the highest margin product of all 20 in the range.

---

## 💼 Experience

**Logistics Operations Associate, JD.com** · Jul 2025 to present

Drivers were working from stop lists with no geographic logic, crossing and re-crossing the same patch all day. I exported the route data and used pivot tables to group 200+ daily stops into postcode clusters, balancing route size against distance so each driver covered one contiguous area. Routes that used to finish between 13:00 and 15:00 now finish around midday, on the same daily volume, against a 15:00 cutoff.

I build and maintain the daily, weekly and monthly reporting that station and regional management read each morning, covering fulfilment, pickup, route performance and complaints. It supported a 99.6% fulfilment rate that ranked the station Top 5 across the EU network, and a 100% pickup rate that took the No. 1 position.

I am also the escalation point for delivery exceptions. Cases come in through the day and we respond inside 30 minutes. Customer service refers one over and I take it from both ends, the driver on the round and the customer on the phone. Address resolution failures, non-receipt claims. The same cases turn up in the complaint data I analyse, so I am not reading a report about something I did not see.

Root cause analysis on that complaint data led to corrective actions that ranked the station Top 10 in the EU on that measure. I also provided the operational analysis behind a pilot third delivery wave, a 19:00 round added on top of the morning and afternoon waves. Ours was the first station in the EU network to run it.

**Data Analyst, Amdari** · Feb 2025 to present

Applied analytics programme, project delivery. Project work on industry datasets, each scoped to a business brief and delivered end to end. The four projects above were delivered through this programme.

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
