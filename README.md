<h1 align="center">Marvellous Umeilechukwu</h1>

<p align="center">
  <strong>Data Analyst</strong><br>
  Data and Operations Analysis
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/marvel7/">LinkedIn</a> ·
  <a href="mailto:marvellousug7@gmail.com">Email</a> ·
  <a href="Marvellous-Umeilechukwu-CV.pdf">CV</a> ·
  London, UK
</p>

---

### The site was certain operator error caused their downtime. 69% of it was not.

![Downtime factor analysis](dashboard.png)

Three analyses below. Each one is published with its raw data, its queries and its
dashboard, so you can check the result instead of taking my word for it.

I came into analysis from inside an operation rather than from outside one. I own the
daily reporting for a last mile delivery station, which means a wrong number is
something I watch happen on the floor that afternoon, not something I find in a review
three weeks later.

---

## 📁 Analytics Projects

Project based analytics on supplied industry datasets, each scoped to a business brief
and delivered end to end.

| Project | Tools | The finding |
|---|---|---|
| [Production Downtime Analysis](https://github.com/Marvllous/greentech-production-downtime-analysis) | SQL Server, Power BI | 69% of downtime was process and supply, not people |
| [Loan Portfolio Risk Analysis](https://github.com/Marvllous/horizon-trust-loan-portfolio-risk-analysis) | Power BI, DAX | The largest exposure and the actual losses sat in different products |
| [Sales and Order Analysis](https://github.com/Marvllous/emerald-springs-sales-analysis) | Excel | Revenue rank and profit rank disagreed |

<br>

### [Production Downtime Analysis](https://github.com/Marvllous/greentech-production-downtime-analysis)
`SQL Server` `Power BI` · Amdari, 2025 to 2026

> **Management had a theory. The data disagreed, and I had to show them why.**

**The data.** 645 production batches at a site losing an estimated $1.5M a year to
unplanned downtime, with no visibility on the cause. Four related tables. The brief
recorded that management assumed operator error was the main driver.

**What I did.** The evidence was unusable as it stood: 13 downtime factor columns
sitting side by side, impossible to group or join to the factor reference table. I
restructured them into rows with UNPIVOT, which let me count downtime by cause for the
first time, then tested the operator-error assumption directly against the reference
table rather than accepting it.

I also refused to rank the ten operators by raw event count. That would have punished
whoever ran the most batches. I measured each operator's delay rate as a proportion of
their own work instead, which separated the people carrying the most volume from the
people genuinely running late.

**What it showed.** 645 batches, 56% of them delayed, 21.74 days of production time
lost. 69% of 885 downtime events came from process and supply rather than operator
error. The corrective focus moved off performance management and onto maintenance
scheduling and material supply.

<br>

### [Loan Portfolio Risk Analysis](https://github.com/Marvllous/horizon-trust-loan-portfolio-risk-analysis)
`Power BI` `DAX` `Power Query` · 10Alytics, 2026

> **The bank could say where its money was. It could not say where its risk was.**

**The data.** 5,000 loans and $636.68M of lending, held in one flat table of 37
columns. No model behind it, so nothing could be grouped, compared or drilled into.

**What I did.** Modelled it into a star schema of one fact table and six dimensions,
testing every key for conflicting attributes before collapsing duplicates. Built a
continuous calendar in DAX, held every measure in a dedicated table, and added a
calculated column bucketing loan ageing into 30 day bands. Delivered a two page
dashboard covering profit and loss, with cross-filtering, slicers and thresholds that
flag themselves.

**What it showed.** 93.8% of the 209 defaults came from one customer segment holding
29% of the lending. Mortgage held 88% of the outstanding balance and under 10% of the
failures, so the largest exposure and the actual losses sat in different products
entirely. Branch lending volume varied 1.4 times across 20 branches while default rate
varied 2.8 times, which moved the question away from lending scale and towards how
credit decisions are made locally.

<br>

### [Sales and Order Analysis](https://github.com/Marvllous/emerald-springs-sales-analysis)
`Excel` · 10Alytics, 2026

> **The most useful thing I found was not a sales finding.**

**The data.** One month of sales and orders for a beverage distributor. 250 orders
across three unlinked tables, inconsistent text fields, dates stored as serial numbers.
Revenue was visible. What drove it was not.

**What I did.** Cleaned and standardised the source, joined all three tables on ID,
then built gross sales, cost, discount and profit at line level. Validated every total
against a control figure before accepting it.

**What it showed.** 250 orders, €12,960.50 gross, 44.4% margin. One sales channel
out-earned two others combined. The largest revenue category ranked near the bottom on
profit per unit, while the smallest category held the highest margin product of all 20
in the range.

That validation check also surfaced nearly 20% of orders sitting in a pending status.
I could size the exposure and rule out the obvious causes, but the data could not tell
me why. I reported it separately from the revenue findings and said so, rather than
inventing a reason that sounded better.

---

## 🔎 How I Work

I write the business question in plain English before I touch a query. What are we
trying to find out, what data answers it, what does the answer look like. Then I
validate every summary figure against a control total before I present it, because a
clean looking dashboard built on an unverified join is worse than no dashboard.

Each of the three projects above publishes its own limitations. That is deliberate. An
analysis that hides where its evidence stops is harder to trust than one that names it.

---

## 🤝 How I Work With People

What I build is read at the start of a shift and acted on before the end of it, so if a
figure is unclear or wrong I find out the same afternoon. That teaches you fast. Nobody
reading before a shift wants method. They want the number, what changed and what to do
about it. A report that needs explaining has already failed.

It also teaches you that the question someone asks is rarely the whole question. People
ask for a figure when what they actually need is a decision, so I find out what the
answer is for before I give it. That one habit has saved more wasted work than any
technique I know.

The last part is being straight about limits. If the data can size a problem but not
explain it, I say so. Analysts lose credibility by filling gaps with something that
sounds plausible, and you only get to do that once.

---

## 🛠 What I Can Do With Data

| Problem | How I handle it |
|---|---|
| **One flat table cannot be analysed** | Model it into a fact table and dimensions, checking every key for conflicting attributes before collapsing it |
| **Raw data is not analysis ready** | Validate the source before transforming it, then restructure wide tables into rows that can be grouped and joined |
| **Nobody knows what is driving a number** | Break the metric down across dimensions until I can isolate the driver, then quantify what it costs |
| **An assumption needs testing, not confirming** | Design the query so it can disprove the belief, then report what it actually shows |
| **A comparison is not like for like** | Build rates rather than raw counts, so volume differences do not distort the ranking |
| **Size is being mistaken for risk** | Separate exposure from failure rate, because the biggest balance and the biggest problem are often different things |
| **Stakeholders cannot read a spreadsheet** | Build dashboards they can filter themselves, so one report answers several people's questions |
| **The numbers need to be trusted** | Validate every figure against a control total before it goes anywhere |

`SQL Server` `PostgreSQL` `Power BI` `Power Query` `DAX` `Excel`

Also working with `Claude` and `ChatGPT` for documentation, review and pressure-testing

<details>
<summary><strong>Specific techniques, and what I used them for</strong></summary>

<br>

**SQL**

| Capability | Applied to |
|---|---|
| **UNPIVOT** | Reshaping 13 wide factor columns into rows that could be grouped and joined |
| **Views** | Holding transformation logic in one place so downstream queries stay clean |
| **CTEs** | Staging validation checks before analysis runs |
| **CASE logic** | Splitting causes into categories so root causes can be attributed properly |
| **COUNT(DISTINCT)** | Building comparable rates across groups of unequal size |
| **DATEDIFF** | Calculating duration variance against planned targets |
| **Multi-table joins** | Linking four related tables through fact and dimension keys |

**Power BI**

| Capability | Applied to |
|---|---|
| **Star schema modelling** | Splitting one flat table of 37 columns into a fact table and six dimensions |
| **Key integrity validation** | Testing every dimension key for conflicting attributes before removing duplicates |
| **DAX measures** | Rates, distinct counts and filtered aggregates that respond to every slicer on the page |
| **Calculated columns** | Bucketing continuous values into bands a business can act on, such as ageing in 30 day periods |
| **DAX date tables** | A continuous calendar so time based visuals do not break on gaps in the source |
| **Relationship management** | Diagnosing an inactive relationship that was silently flattening a chart, then repairing it |
| **Conditional formatting by measure** | Letting thresholds flag themselves as the data changes, rather than colouring by hand |
| **Decomposition trees** | Drilling exposure through product, segment, geography and branch type in one visual |

</details>

---

## 💼 Experience

**Logistics Operations Associate, JD.com** · Jul 2025 to present

I build and maintain the daily operational reporting for a delivery station, covering
fulfilment rate, pickup rate, route efficiency and complaint data. The station reached
a 99.6% fulfilment rate, ranking Top 5 in Europe, and a 100% pickup rate that took the
No. 1 position EU-wide.

The reporting also found a problem nobody had raised. Drivers were working from
allocation lists with no geographic logic, so I grouped 200+ daily stops into postcode
clusters, balancing route size against distance. Routes that ran to between 13:00 and
15:00 now finish around midday on the same volume.

Ran root cause analysis on customer complaint data and used the findings to drive
corrective actions, which ranked the station Top 10 across the EU on that measure.

---

## 🎓 Background

**MSc Project Management**, Ravensbourne University, London

**LLB Law**, Igbinedion University, Nigeria

**Training**
- 10Alytics, applied data analytics programme, 2026
- Amdari, applied data analytics programme, 2025 to 2026

**Certifications**
- Google Data Analytics Professional Certificate
- Supply Chain Logistics, Rutgers University via Coursera

---

## 📬 Contact

**Email:** marvellousug7@gmail.com

**LinkedIn:** [linkedin.com/in/marvel7](https://www.linkedin.com/in/marvel7/)

**CV:** [View my CV](Marvellous-Umeilechukwu-CV.pdf)
