
# Coffee Heaven — 2023 Half-Time Sales Review (Power BI)


A one-page Power BI dashboard for a café chain that highlights **Total Sales**, **Top Products**, **Store Comparisons (Miami/Orlando/Tampa)**, **Peak Hours**, and a **Full-Year Forecast**, built on **AWS S3 and Snowflake**.


---

## Dashboard
- **Dashboard (view/download):** https://drive.google.com/file/d/1I4pgKQFayISlbFtzcJkFHP840umSqktY/view?usp=sharing

![Image](https://github.com/user-attachments/assets/1aa84a67-dffc-420b-98d5-a183ef9b4693)



## Table of Contents
- [About the Project](#about-the-project)
- [Dataset (Synthetic)](#dataset-synthetic)
- [Business Questions](#business-questions)
- [Features & KPIs](#features--kpis)
- [Steps Followed](#steps-followed)
- [Contact](#contact)

---

##  About the Project

**Goal:** Present a **mid-year executive review** for Coffee Heaven’s Florida region—sales trends, peak hours, and top products across **three locations**.  
**Tech:** Power BI · DAX · AWS S3 · Snowflake · Excel · Smart Narratives.  
**Brand:** **Coffee Heaven** (Portfolio Dataset).

---

##  Dataset 


Key tables used:
Fact Sales · Store Dim · Product Dim · Date Dim  

Columns: `TransactionDate`, `Hour`, `Store`, `Product`, `Category`, `UnitPrice`, `Qty`, `TotalSales`.  
> Data staged on **AWS S3**, modeled via **Snowflake**, then consumed in **Power BI**.

---

## Business Questions  

1. How is **Coffee Heaven** performing at **mid-year 2023** across its three **Florida stores** (**Miami**, **Orlando**, and **Tampa**)?  
2. Which **products** and **categories** generate the highest **sales volume** and **revenue**?  
3. What are the **peak sales hours** and **days**, and how do they differ by **location**?  
4. What is the **average order size** and **transaction frequency trend (YTD)**?  
5. How close are we to our **full-year sales goal**, and what can we forecast for **H2 2023 (Jul–Dec)**?  
6. Which insights can help **store managers** and **leadership** optimize **staffing**, **menu mix**, and **promotion timing**?  


---

## Features & KPIs  
- **Executive KPI Panel:** **Total Sales**, **Transactions**, **Average Order Size**, **Stores**, and **Best Sellers (Revenue & Quantity)**.  
- **Top Products & Categories:** Ranked by **Revenue** with **custom labels** and **currency formatting**.  
- **Time-of-Day / Day-of-Week Heatmaps:** Identify **peak hours** and **sales patterns** by store.  
- **Forecast Section:** Dynamic **running total projection** for **H2 2023** based on **average daily sales**.  
- **Store-Level Comparison Cards:** Track **growth and performance** across **Miami**, **Orlando**, and **Tampa**.  
- **Smart Narrative Summaries:** Auto-generated **plain-English insights** and **calls to action** for leadership.  
- **Infographic-style Power BI Layout:** Designed with **Coffee Heaven’s warm color palette** and **executive presentation theme**.  

---

## Steps Followed  

**1) Data Pipeline & Modeling**  
- Connected raw sales data stored on **AWS S3**, processed via **Snowflake**, and imported into **Power BI**.  
- Built a **Star Schema Model** with **Fact Sales** and **Dimension tables** for **Date**, **Store**, and **Product**.  
- Created calculated columns for **Hour of Sale**, **Time of Day (Morning/Afternoon/Evening)**, and **Month Short** for sorting.  

**2) Core DAX Measures**  
- Created measures for **Total Sales**, **Transactions**, **Average Order Size**, **% of Sales**, and **Ranking**.  
- Used `ALLSELECTED`, `SWITCH`, and `CALCULATE` for **context-aware forecasting** and **dynamic visuals**.  

**3) Visual Design & Layout**  
- Created infographic canvas in **PowerPoint** and imported into **Power BI**.  
- Added **bar charts**, **matrix tables**, **heatmaps**, and **forecast curves** per store.  
- Applied **conditional formatting** and a branded warm palette (`#A1343C – #652C23`).  

**4) Forecast & Narrative**  
- Built a **Forecast Date Table** using `CALENDAR()` extending through **Dec 2023**.  
- Created **Average Daily Sales** and **Running Total** measures for projection.  
- Integrated **Smart Narrative Visual** to summarize **Q1 vs Q2** performance and predict **FY targets**.  

**5) Presentation & Deployment**  
- Refined layout for **executive readability** and simplified KPI visuals.  
- Published to **Power BI Service** for **leadership review**, **tracking**, and **PDF exports**.  

---

## Outcome  
A visually rich **Power BI dashboard** serving as **Coffee Heaven’s 2023 Half-Time Review**, combining **data-driven storytelling** with **business insights**.  
It empowers leadership to **evaluate progress**, **optimize store operations**, and **forecast growth** across all three **Florida locations** with clarity and confidence.  





---



