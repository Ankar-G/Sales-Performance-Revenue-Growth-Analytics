# Sales & Marketing Analytics Dashboard

> A four-page, interactive Power BI report that tracks revenue, profitability, product mix, regional and sales-representative performance, and customer behavior.

![Status](https://img.shields.io/badge/Status-Portfolio%20Project-blue)
![Tool](https://img.shields.io/badge/Tool-Power%20BI-F2C811)
![Dashboards](https://img.shields.io/badge/Dashboards-4-1f77b4)

**Evidence legend used throughout this document**

| Label | Meaning |
|---|---|
| **Verified** | Read directly from the dashboard screenshots |
| **Derived** | Calculated by me from rounded values shown on the dashboards (small rounding differences are expected) |
| **[PLACEHOLDER: confirm this information]** | Not visible in the screenshots; must be confirmed against the actual `.pbix` file or dataset |

> **Tool note:** The screenshots show Power BI report features (page navigator, slicers, cross-filtering visuals), so this README assumes **Power BI**. **[PLACEHOLDER: confirm this information]**

---

## Table of Contents

1. [Project Overview](#1-project-overview)
2. [Problem Statement](#2-problem-statement)
3. [Business Objectives](#3-business-objectives)
4. [Project Workflow](#4-project-workflow)
5. [Dataset and Data Model](#5-dataset-and-data-model)
6. [Data Cleaning and Preparation](#6-data-cleaning-and-preparation)
7. [Key Calculations and Metrics](#7-key-calculations-and-metrics)
8. [Dashboard Overview](#8-dashboard-overview)
9. [Dashboard 1: Executive Sales Overview](#9-dashboard-1-executive-sales-overview)
10. [Dashboard 2: Product Performance Analysis](#10-dashboard-2-product-performance-analysis)
11. [Dashboard 3: Regional & Sales Representative Performance](#11-dashboard-3-regional--sales-representative-performance)
12. [Dashboard 4: Customer & Revenue Analysis](#12-dashboard-4-customer--revenue-analysis)
13. [Key Project Insights](#13-key-project-insights)
14. [Business Value](#14-business-value)
15. [Business Questions Answered](#15-business-questions-answered)
16. [Technical Skills and Tools](#16-technical-skills-and-tools)
17. [Project Structure](#17-project-structure)
18. [Data Validation Notes](#18-data-validation-notes)
19. [Dashboard Preview](#19-dashboard-preview)
20. [Connect With Me](#20-connect-with-me)

---

## 1. Project Overview

**Sales & Marketing Analytics** is a four-page interactive Power BI report that turns sales data into decision-ready views for executives, product managers, regional sales leaders, and account managers.

| Item | Detail |
|---|---|
| **Reporting period** | Monthly and quarterly views span January–December; the calendar vs. fiscal year and the Year slicer values are **[PLACEHOLDER: confirm this information]** |
| **Headline results (all filters = "All")** | Revenue **25.08M**, Profit **8.40M**, Profit Margin **33.49%**, Orders **8,818**, Customers **900**, Sales Representatives **40** |
| **Currency** | KPI cards show no currency symbol; insight text uses "$". **[PLACEHOLDER: confirm this information]** |
| **Report pages** | Executive Sales Overview · Product Performance Analysis · Regional & Sales Representative Performance · Customer & Revenue Analysis |
| **Navigation** | Left-hand page navigator on every page plus page-specific slicers |

---

## 2. Problem Statement

Sales leadership needs one place to answer: *How is the business performing, what is driving it, and where should we act?* Without a consolidated view, leaders cannot easily see:

- Whether growth and margin are healthy across time periods.
- Which products, categories, regions, and representatives generate (or dilute) profit.
- How dependent revenue is on a few categories, segments, industries, or accounts.
- Whether customers are being retained.

---

## 3. Business Objectives

1. Monitor revenue, profit, margin, growth, and order volume in a single executive view.
2. Identify top and bottom products and categories by revenue, profit, and units sold.
3. Compare regional and sales-representative performance and assess target attainment.
4. Understand customer segments, key accounts, industries, and retention.
5. Surface data-quality and metric-definition issues before the report is used for decisions (see [Section 18](#18-data-validation-notes)).

---

## 4. Project Workflow

| Step | Activity | Status |
|---|---|---|
| 1 | Define KPIs and dashboard pages | Reflected in the report |
| 2 | Acquire and profile source data | **[PLACEHOLDER: confirm this information]** |
| 3 | Clean and transform data | **[PLACEHOLDER: confirm this information]** |
| 4 | Build the data model and relationships | **[PLACEHOLDER: confirm this information]** |
| 5 | Create measures (revenue, profit, margin, growth, AOV, etc.) | Reflected in the report; exact logic **[PLACEHOLDER: confirm this information]** |
| 6 | Design four report pages with slicers and navigation | Reflected in the report |
| 7 | Add written key insights to each page | Reflected in the report |
| 8 | Validate totals and definitions across pages | Documented in [Section 18](#18-data-validation-notes) |

---

## 5. Dataset and Data Model

The underlying dataset and data model were **not inspected** for this README. Tables, keys, and relationships must be added after review of the source file.

### 5.1 Fields observable in the dashboards

| Field / Entity | Where it appears | Likely role (inferred) |
|---|---|---|
| `Year` | Slicer on all pages | Date attribute |
| `Month_Name` | Slicer on pages 2–4; monthly charts | Date attribute |
| `Region_Name` | Slicer on pages 1, 3, 4; regional charts | Geography attribute (12 regions implied; see below) |
| `Category` | Slicer on page 1; category charts | Product attribute (Technology, Furniture, Office Supplies) |
| `Customer_Segment` | Slicer on page 1; segment charts | Customer attribute (Enterprise, Mid-Market, Small Business) |
| `Sales_Rep_Name` | Slicer on page 2; representative charts | Sales team attribute (40 representatives) |
| Product name | Product charts | Product attribute |
| Customer name, Industry | Customer charts | Customer attributes |
| Revenue, Profit, Orders, Units, Sales Target | KPI cards / chart legends | Measures or numeric fields |

Regions identified in the screenshots: West Coast, Florida Peninsula, Texas Gulf, New York Metro, Pacific Northwest, Carolinas, Mid-Atlantic, Midwest Central, Southeast, New England, Mountain West, Great Lakes. Mountain West and Great Lakes are visible only in the Dashboard 3 table; the Dashboard 1 and 3 region bar charts are scrollable and show the top regions.

### 5.2 Data model (to be completed)

| Item | Status |
|---|---|
| Fact table(s) | **[PLACEHOLDER: confirm this information]** |
| Dimension tables (Date, Product, Customer, Region, Sales Rep) | **[PLACEHOLDER: confirm this information]** |
| Primary / foreign keys | **[PLACEHOLDER: confirm this information]** |
| Relationship cardinality and filter direction | **[PLACEHOLDER: confirm this information]** |
| Where Sales Target is stored and at what grain | **[PLACEHOLDER: confirm this information]** |
| Data source (file, database, synthetic generator) | **[PLACEHOLDER: confirm this information]** |

---

## 6. Data Cleaning and Preparation

No cleaning steps are documented here because none can be verified from the screenshots. Complete this table from the Power Query / source-file review.

| Area | Step performed | Status |
|---|---|---|
| Missing values | — | **[PLACEHOLDER: confirm this information]** |
| Duplicates | — | **[PLACEHOLDER: confirm this information]** |
| Data types and formats | — | **[PLACEHOLDER: confirm this information]** |
| Date table / month sorting | — | **[PLACEHOLDER: confirm this information]** (see validation notes V-07, V-13) |
| Derived columns (profit, quarter, etc.) | — | **[PLACEHOLDER: confirm this information]** |

---

## 7. Key Calculations and Metrics

> **Reference examples only.** The DAX below shows standard ways to compute each KPI. Table and column names (`Sales`, `Customers`, etc.) are placeholders and the actual measures have **not** been verified. **[PLACEHOLDER: confirm this information]**

### 7.1 KPI definitions

| KPI | Definition | Displayed value | Appears on |
|---|---|---|---|
| Total Revenue | Sum of sales revenue | 25.08M | Pages 1, 2 (as Product Revenue), 3 |
| Total Profit | Sum of profit | 8.40M | Page 1 |
| Profit Margin % | Total Profit ÷ Total Revenue | 33.49% | Pages 1, 2 |
| Revenue Growth % | Period-over-period change in revenue (period undefined) | 10.00% | Page 1 |
| Total Orders | Count of distinct orders | 8,818 | Page 1 |
| Total Units Sold | Sum of quantity | 130K | Page 2 |
| Average Order Value | Total Revenue ÷ Total Orders | 2.84K | Page 4 |
| Revenue per Customer | Total Revenue ÷ Distinct customers | 27.86K | Page 4 |
| Repeat Purchase Rate % | Repeat customers ÷ Total customers | 92.33% | Page 4 |
| Avg. Revenue per Representative | Total Revenue ÷ Distinct sales representatives | 626.90K | Page 3 |

### 7.2 Reference DAX

```DAX
-- Revenue, profit, margin
Total Revenue = SUM ( Sales[Revenue] )
Total Profit  = SUM ( Sales[Profit] )
Profit Margin % = DIVIDE ( [Total Profit], [Total Revenue] )

-- Orders, units, order value
Total Orders     = DISTINCTCOUNT ( Sales[Order_ID] )
Total Units Sold = SUM ( Sales[Quantity] )
Average Order Value = DIVIDE ( [Total Revenue], [Total Orders] )

-- Customers
Total Customers = DISTINCTCOUNT ( Sales[Customer_ID] )
Revenue per Customer = DIVIDE ( [Total Revenue], [Total Customers] )

-- Repeat purchase rate (definition of "repeat" must be confirmed)
Repeat Customers =
CALCULATE (
    DISTINCTCOUNT ( Sales[Customer_ID] ),
    FILTER (
        VALUES ( Sales[Customer_ID] ),
        CALCULATE ( DISTINCTCOUNT ( Sales[Order_ID] ) ) > 1
    )
)
Repeat Purchase Rate % = DIVIDE ( [Repeat Customers], [Total Customers] )

-- Sales representatives
Total Sales Representatives = DISTINCTCOUNT ( Sales[Sales_Rep_ID] )
Avg Revenue per Representative = DIVIDE ( [Total Revenue], [Total Sales Representatives] )

-- Revenue growth: requires a defined comparison period (YoY, QoQ, MoM)
Revenue Growth % =
VAR Prior = CALCULATE ( [Total Revenue], DATEADD ( 'Date'[Date], -1, YEAR ) )
RETURN DIVIDE ( [Total Revenue] - Prior, Prior )
```

### 7.3 Sales target achievement

Target Achievement % should be calculated only when **actual revenue and target use the same period, entity, and aggregation level**:

```DAX
Target Achievement % = DIVIDE ( [Total Revenue], [Total Sales Target] )
```

On the current dashboards, representative revenue (about 0.97M–1.43M) and target labels (about 19K–37K) differ by roughly 28×–52× (Derived), and the achievement chart shows unitless values of 46–55. The target definition therefore requires validation before any attainment claim is made (see V-09).

---

## 8. Dashboard Overview

| # | Dashboard | Slicers (as shown) | Primary audience | Focus |
|---|---|---|---|---|
| 1 | Executive Sales Overview | Year, Region_Name, Category, Customer_Segment | Executives | Revenue, profit, growth, orders |
| 2 | Product Performance Analysis | Year, Month_Name, Sales_Rep_Name | Product / merchandising | Product revenue, profit, units, category trends |
| 3 | Regional & Sales Representative Performance | Year, Month_Name, Region_Name | Sales leadership | Region and representative results, target achievement |
| 4 | Customer & Revenue Analysis | Year, Month_Name, Region_Name | Account / customer success | Segments, key accounts, industries, retention |

---

## 9. Dashboard 1: Executive Sales Overview

**Purpose (as stated on the page):** Track overall sales performance, profitability, and growth across the business.

### KPI cards (Verified)

| KPI | Value |
|---|---|
| Total Revenue | 25.08M |
| Total Profit | 8.40M |
| Profit Margin | 33.49% |
| Revenue Growth | 10.00% |
| Total Orders | 8,818 |

### Charts

| Chart | Type | What it shows |
|---|---|---|
| Revenue & Profit by Quarter | Clustered column | Q1 5.9M / 1.9M · Q2 6.1M / 2.0M · Q3 5.6M / 2.0M · Q4 7.5M / 2.5M (revenue / profit) |
| Revenue by Region | Horizontal bar (scrollable) | West Coast 2.9M, Florida Peninsula 2.8M, Texas Gulf 2.5M, New York Metro 2.4M, Pacific Northwest 2.2M, Carolinas 2.1M, Mid-Atlantic 2.1M, Midwest Central 1.9M, Southeast 1.9M, New England 1.6M |
| Revenue by Product Category | Horizontal bar | Technology 19.5M, Furniture 3.8M, Office Supplies 1.7M |
| Monthly Revenue & Profit Trend | Line | Revenue ranges from 1.7M (July) to 2.8M (December); profit from 0.6M to 1.0M |
| Actual Sales vs Sales Target | Area | Single series with values 915 down to 627; **see V-02** |

### Key insights

1. **Q4 is the strongest quarter.** Q4 revenue of 7.5M is about 29.9% of annual revenue (Derived) and about 34% above Q3 (Derived). Monthly revenue rises from 1.7M in July to 2.8M in December.
2. **Margin is stable.** Quarterly margins calculated from the displayed values stay in a narrow range of about 32%–36% (Derived), consistent with the 33.49% overall margin.
3. **Technology dominates.** Technology contributes 19.5M, about 77.7% of revenue (Derived).

### Recommendations

- Treat Technology concentration as a portfolio risk and test growth in Furniture and Office Supplies.
- Plan inventory, staffing, and promotions around the Q4 peak and investigate the July trough.
- Do not use the Revenue Growth card or the "Actual Sales vs Sales Target" chart for decisions until their definitions are confirmed (V-01, V-02).

---

## 10. Dashboard 2: Product Performance Analysis

**Purpose (as stated on the page):** Analyze product-wise sales, profitability, and trends to identify top performers and growth opportunities.

### KPI cards (Verified)

| KPI | Value |
|---|---|
| Total Unit Sold | 130K |
| Total Selling Product (label as shown) | Productivity Suite License |
| Product Revenue | 25.08M |
| Product Profit Margin % | 33.49% |

### Charts

| Chart | Type | What it shows |
|---|---|---|
| Revenue by Product | Horizontal bar (scrollable) | ProBook 15 Performance Laptop 3.0M, ProBook 14 Business Laptop 2.8M, Productivity Suite License 1.6M, Endpoint Security License 1.4M, Workstation Elite 16 Laptop 1.3M, UltraSlim 13 Laptop 1.2M, 27-inch QHD Monitor 1.0M, Cloud Backup Subscription 1.0M, Project Management Platform License 0.9M |
| Profit by Product Category | Column | Technology 6.6M, Furniture 1.3M, Office Supplies 0.5M |
| Units Sold by Category | Column | Technology 83K, Office Supplies 31K, Furniture 16K |
| Revenue vs Profit by Product | Clustered bar | Laptops show high revenue with low profit (about 0.4M profit on 3.0M and 2.8M revenue); Productivity Suite License (1.6M revenue, 1.1M profit) and Endpoint Security License (1.4M revenue, 1.0M profit) show high profit. Some data labels overlap |
| Monthly Product Category Trends | Line (3 series) | Technology fluctuates between about 1.2M and 2.2M per month; Furniture and Office Supplies stay roughly between 0.1M and 0.4M |

### Key insights

1. **Technology drives volume and profit.** It accounts for 83K of 130K units (about 64%) and 6.6M of 8.4M profit (about 79%) (Derived).
2. **Revenue leaders are not profit leaders.** The two ProBook laptops lead revenue but convert only about 13–14% of revenue to profit (Derived), while software licenses convert roughly 69–71% (Derived). The dashboard's own insight also flags products with low or negative profitability.
3. **Office Supplies is high-volume, low-value.** It sells 31K units (about twice Furniture's 16K) but generates only 1.7M revenue and 0.5M profit, a margin of about 29% versus about 34% for the other categories (Derived).

### Recommendations

- Review pricing and cost structure for high-revenue, low-margin laptops.
- Evaluate bundling high-margin licenses and subscriptions with hardware sales.
- Identify the specific products with negative profit (Workstation Elite 16 Laptop appears to show a negative profit label; verify) and decide on repricing or rationalization.

> The Key Insights card on this page is partially covered by a tooltip in the screenshot, so the first insight is only partly legible.

---

## 11. Dashboard 3: Regional & Sales Representative Performance

**Purpose (as stated on the page):** Track revenue, performance, and target achievement across regions and sales representatives.

### KPI cards (Verified)

| KPI | Value |
|---|---|
| Total Revenue | 25.08M |
| Top Performing Region | West Coast |
| Total Sales Representative | 40 |
| Avg. Revenue per Representative | 626.90K |

### Charts

| Chart | Type | What it shows |
|---|---|---|
| Revenue by Region | Horizontal bar | Same regional ranking as Dashboard 1 |
| Actual Sales VS Sales By Representative (title as shown) | Bar with two series | Revenue: Jennifer Rivera 1.43M, Tyler Fisher 1.27M, Jennifer Ortiz 1.27M, Jason Rivera 1.14M, Susan Zimmerman 1.12M, Laura Young 1.09M, Patrick Grant 1.02M, Hannah Rivera 0.97M. Target labels shown: 28K, 37K, 25K, 24K, 32K, 21K, 37K, 19K respectively |
| Representative Target Achievement | Horizontal bar | Unitless values: David Lopez 55, Laura Young 53, Hannah Rivera 52, Jennifer Ortiz 52, Jennifer Rivera 51, Brian Morgan 48, Jason Rivera 48, Sofia Ortiz 47, Grace Walker 46 |
| Regional Profitability | Horizontal bar | Profit: West Coast 956.18K, Florida Peninsula 934.1K, Texas Gulf 836.26K, Pacific Northwest 802.57K, New York Metro 796.58K, Carolinas 686.3K, Midwest Central 663.39K, Mid-Atlantic 643.7K, Southeast 627.82K |
| Monthly Regional Sales Trend | Matrix table (scrollable) | Revenue by month and region. Visible region totals: Carolinas 2,145,817.80; Florida Peninsula 2,816,094.55; Great Lakes 1,126,679.70; Mid-Atlantic 2,128,842.55; Midwest Central 1,909,355.25; Mountain West 1,398,115.00; New England 1,643,042.25; New York Metro 2,421,375.50; Pacific Northwest 2,228,259.70 |

### Key insights

1. **West Coast leads, and the gap to the bottom is wide.** West Coast earns 2.9M revenue and 956.18K profit. From the table totals, Great Lakes (about 1.13M) and Mountain West (about 1.40M) are the lowest regions, with Great Lakes at roughly 39% of West Coast revenue (Derived).
2. **Top representatives far exceed the average.** Jennifer Rivera's 1.43M is about 2.3× the 626.90K average (Derived), and all eight representatives shown exceed the average. Because 40 representatives exist, revenue concentration among top performers should be checked.
3. **Regional monthly revenue is volatile.** For example, Carolinas moves from 8,028.60 in March to 614,553.30 in April, and Great Lakes shows 1,079.85 in May. This may indicate lumpy deals or a data-grain issue (see V-10).

### Recommendations

- Investigate Great Lakes and Mountain West for pipeline, coverage, or pricing gaps.
- Review whether top-representative results reflect territory advantage or repeatable practices.
- Define the sales-target methodology (period, grain, units) before using target-achievement figures in performance reviews.

---

## 12. Dashboard 4: Customer & Revenue Analysis

**Purpose (as stated on the page):** Understand customer segments, key accounts, and revenue trends to identify growth opportunities and improve customer retention.

### KPI cards (Verified)

| KPI | Value |
|---|---|
| Total Customer | 900 |
| Avg. Order Value | 2.84K |
| Revenue per Customer | 27.86K |
| Repeat Purchase Rate | 92.33% |

### Charts

| Chart | Type | What it shows |
|---|---|---|
| Revenue by Customer Segment | Column | Enterprise 12.0M, Mid-Market 9.1M, Small Business 4.0M |
| Top 10 Customers by Revenue | Horizontal bar (scrollable) | Hudson Consulting Group 0.45M, Franklin Freight Lines 0.41M, Dunmore Health Partners 0.40M, Copperfield Systems 0.34M, Paragon Systems 0.33M, Valley Medical Group 0.32M, Trailhead Capital Advisors 0.31M, Zenith Freight Lines 0.28M, Elmhurst Systems 0.27M (10th not visible) |
| New vs Repeat Customers | Donut | Repeat 831 (92.33%), New 69 (7.67%), total 900 |
| Revenue by Industry | Horizontal bar | Healthcare 3.9M, Technology 3.6M, Manufacturing 3.2M, Logistics 2.9M, Retail 2.5M, Financial Services 2.3M, Government & Nonprofit 2.3M, Professional Services 2.1M, Construction 1.4M, Education 0.9M |
| Monthly Revenue Trends by Customer Segment | Overlapping area | Enterprise, Mid-Market, Small Business by month; month axis is not in calendar order (see V-13) |

### Key insights

1. **Enterprise is the core segment.** Enterprise generates 12.0M, about 47.8% of revenue; Mid-Market contributes about 36.3% and Small Business about 15.9% (Derived).
2. **Retention appears strong.** 831 of 900 customers (92.33%) are classified as repeat, and the average customer places about 9.8 orders (8,818 ÷ 900, Derived). The "repeat" definition still needs confirmation (V-14).
3. **Industry mix is led by Healthcare, with low account concentration.** Healthcare contributes 3.9M (about 15.5%), and the top three industries together contribute about 42.7% (Derived). The largest visible customer (0.45M) is only about 1.8% of revenue, so revenue is not dependent on any single account (Derived).

### Recommendations

- Build retention and expansion plans for the top accounts and Enterprise segment.
- Test targeted growth offers for Small Business, the smallest segment.
- Consider vertical-specific campaigns for Healthcare and Technology, and review under-penetrated industries such as Education and Construction.

---

## 13. Key Project Insights

| Theme | Finding | Evidence |
|---|---|---|
| Growth timing | Revenue builds through the year and peaks in Q4 (7.5M) and December (2.8M) | Verified |
| Profitability | Overall margin is 33.49%; category margins are about 29%–34% | Verified / Derived |
| Category concentration | Technology provides about 78% of revenue and about 79% of profit | Derived |
| Product quality of revenue | Top-revenue laptops have thin margins; software licenses have high margins | Verified / Derived |
| Regional spread | West Coast (2.9M) vs. Great Lakes (about 1.13M) | Verified / Derived |
| Customer base | 900 customers, 92.33% repeat, Enterprise about 48% of revenue | Verified / Derived |

---

## 14. Business Value

- **Executives** get a consistent view of revenue, margin, and seasonality.
- **Product teams** can see where volume does not translate to profit and prioritize pricing and cost reviews.
- **Sales leaders** can compare regions and representatives and identify coverage gaps.
- **Account teams** can focus on key accounts, segments, and industries and monitor retention.
- **Analytics governance** is supported by documenting metric-definition questions rather than hiding them.

---

## 15. Business Questions Answered

| Dashboard | Questions |
|---|---|
| Executive Sales Overview | How much revenue and profit did we generate? Is margin stable? Which quarter, region, and category contribute most? How does revenue trend by month? |
| Product Performance | Which products and categories sell the most units and revenue? Which are the most and least profitable? How do category sales trend by month? |
| Regional & Sales Rep | Which region leads? How many representatives do we have and what is average revenue per representative? Who are the top representatives? Which regions are most profitable? How does monthly revenue vary by region? |
| Customer & Revenue | How many customers do we have? What is the average order value and revenue per customer? How many customers are repeat vs. new? Which segments, industries, and accounts generate the most revenue? |

---

## 16. Technical Skills and Tools

| Area | Skills / tools |
|---|---|
| BI tool | Power BI (inferred from the report interface; **[PLACEHOLDER: confirm this information]**) |
| Calculations | KPI design, ratio measures, DAX (reference examples; actual measures **[PLACEHOLDER: confirm this information]**) |
| Visualization | Column, bar, line, area, donut, KPI cards, matrix table, slicers, page navigation |
| Analytics | Revenue and profitability analysis, product mix analysis, regional and representative benchmarking, customer segmentation, retention analysis |
| Data quality | Cross-page reconciliation, metric-definition review, chart-design review |
| Communication | Embedded key-insight summaries for business audiences |

---

## 17. Project Structure

> Folder and file names below are a proposed layout. Mark each as confirmed once it exists in the repository. **[PLACEHOLDER: confirm this information]**

```text
sales-marketing-analytics/
│
├── README.md
│
├── data/                                   # [PLACEHOLDER] raw / processed data files
│   └── sales_data.xlsx                     # [PLACEHOLDER] filename unverified
│
├── dashboard/
│   └── Sales_Marketing_Analytics.pbix      # [PLACEHOLDER] filename unverified
│
├── images/
│   ├── dashboard_1_executive_sales_overview.png
│   ├── dashboard_2_product_performance.png
│   ├── dashboard_3_regional_sales_performance.png
│   └── dashboard_4_customer_revenue_analysis.png
│
└── docs/                                   # [PLACEHOLDER] optional: data dictionary, measure list
```

---

## 18. Data Validation Notes

This section records observations from the four screenshots. **No issue below is claimed to be fixed.** Items marked *Open* require review of the underlying report and data.

### 18.1 Checks that reconcile

| Check | Result |
|---|---|
| Profit ÷ Revenue = 8.40M ÷ 25.08M | 33.49% matches the KPI |
| Quarterly revenue (5.9 + 6.1 + 5.6 + 7.5) and profit (1.9 + 2.0 + 2.0 + 2.5) | About 25.1M and 8.4M; match totals within rounding |
| Category revenue (19.5 + 3.8 + 1.7) | About 25.0M; matches within rounding |
| Category profit (6.6 + 1.3 + 0.5) | 8.4M; matches |
| Category units (83K + 31K + 16K) | 130K; matches |
| Region revenue (12 regions, including Great Lakes and Mountain West from the Dashboard 3 table) | About 25.1M; matches within rounding |
| Region totals in the Dashboard 3 table vs. region bars | Match for all regions visible in both |
| Revenue per representative (25.08M ÷ 40) | About 627.0K vs. 626.90K shown; matches within rounding |
| Average order value (25.08M ÷ 8,818) | About 2,844; matches 2.84K |
| Revenue per customer (25.08M ÷ 900) | About 27.87K vs. 27.86K shown; matches within rounding |
| Repeat rate (831 ÷ 900) and new rate (69 ÷ 900) | 92.33% and 7.67%; match |
| Customer segment (12.0 + 9.1 + 4.0) and industry (sum of 10 values) | About 25.1M each; match within rounding |
| Dashboard 4 segment values for December (1.38 + 0.94 + 0.45) vs. Dashboard 1 December (2.8M) | About 2.77M; matches |

### 18.2 Open issues

| ID | Dashboard | Observation | Why it matters | Status |
|---|---|---|---|---|
| V-01 | 1 | Revenue Growth shows exactly **10.00%** with no comparison period or baseline. | Exact round values can indicate a hard-coded, placeholder, or poorly defined measure. | Open |
| V-02 | 1 | "Actual Sales VS Sales Target" has a single series, no legend, no units, and no visible target. Values (915 down to 627) are sorted by value, not by month, so months appear out of order. The 12 values sum to about 8,827, close to Total Orders (8,818), which suggests the chart may show monthly order counts rather than sales vs. target. | Title, data, and sort order may not match; an area chart is also a poor fit for ranked categories. | Open |
| V-03 | 1 vs 2 | Dashboard 2 shows Technology revenue of about 2.2M in August, higher than total August revenue of 1.9M on Dashboard 1. December Technology (1.4M) plus the other two categories (about 0.6M) is about 2.0M vs. 2.8M on Dashboard 1. Annual totals reconcile, and Dashboard 4 monthly segment values match Dashboard 1. | The monthly category chart on Dashboard 2 may use a different date field, filter, or month mapping. | Open |
| V-04 | 2 | KPI is labeled "Total Selling Product" (likely "Top Selling Product") and shows Productivity Suite License, while Revenue by Product ranks ProBook 15 Performance Laptop first and the page insight calls it the top-revenue product. | The KPI likely ranks by units, but the basis is not labeled. | Open |
| V-05 | 2 | Typos in titles: "Revenue By Porduct", "Profit By Product Caregory", "Total Unit Sold". | Professional polish. | Open |
| V-06 | 2 | Revenue vs Profit by Product has overlapping data labels, and Workstation Elite 16 Laptop appears to carry a negative profit label while the axis starts at 0. The insight mentions "low or negative" profitability without naming products. | Negative values are hard to read and unverified. | Open |
| V-07 | 2 | Key Insights card is partially covered by a tooltip in the screenshot. | Text could not be fully verified. | Open |
| V-08 | 3 | Chart title reads "Actual Sales VS Sales By Representative" (likely "Sales Target"). | Misleading label. | Open |
| V-09 | 3 | Representative revenue (0.97M–1.43M) and target labels (19K–37K) differ by about 28×–52×. "Representative Target Achievement" shows unitless values (46–55) that cannot be reconciled with those figures. The top achiever (David Lopez, 55) is not among the top revenue representatives shown. | Targets may be monthly or per-order while revenue is annual, or achievement may use another formula. Do not publish attainment percentages until period and grain are confirmed. | Open |
| V-10 | 3 | "Monthly Regional Sales Trend" is a scrollable matrix table, not a trend visual, and the July row and several region columns are cut off. Monthly values swing widely (e.g., Carolinas 8,028.60 in March, 614,553.30 in April). | Trend is hard to read; volatility should be confirmed as real rather than a data-grain issue. | Open |
| V-11 | 3 | "Regional Profitability" shows absolute profit, not margin. Pacific Northwest profit (802.57K) exceeds New York Metro (796.58K) despite lower revenue (2.2M vs. 2.4M). | Absolute profit hides margin differences. | Open |
| V-12 | 1, 2, 3 | Revenue by Region appears on both Dashboard 1 and 3; Total Revenue (25.08M) and profit margin (33.49%) repeat across pages. | Duplicate visuals add little; consider replacing with new analysis. | Open |
| V-13 | 4 | Monthly Revenue Trends by Customer Segment lists months out of calendar order (December, November, October, June, March, January, April, September, May, August, February, July) and uses overlapping filled areas. Dashboard 1 uses January–December order. | Trend direction cannot be read reliably; inconsistent sorting between pages. | Open |
| V-14 | 4 | Repeat Purchase Rate (92.33%) has no definition. The measure also sits on a page with Year and Month slicers. | The result of "repeat" classification may change with filters. | Open |
| V-15 | 4 | Top 10 Customers chart shows nine bars without scrolling. | Tenth customer not verified. | Open |
| V-16 | All | KPI cards show no currency or unit labels, while insight text uses "$". | Ambiguous units. | Open |
| V-17 | All | Slicers differ by page (e.g., Category and Customer_Segment only on Dashboard 1; Sales_Rep_Name only on Dashboard 2). Cross-page slicer sync and filter behavior were not tested. | Consistent filtering across pages is unverified. | Open |
| V-18 | 2, 3, 4 | Colors are reused for different meanings (orange is Technology on Dashboard 2, Small Business on Dashboard 4, and Revenue by Region on Dashboard 3). | Can mislead cross-page comparison. | Open |

---

## 19. Dashboard Preview

> Image paths are proposed. Add the screenshots to the `images/` folder with these filenames (or update the paths).

### Dashboard 1: Executive Sales Overview
![Executive Sales Overview dashboard showing revenue, profit, margin, growth, orders, quarterly, regional, category, and monthly trends](https://github.com/Ankar-G/Sales-Performance-Revenue-Growth-Analytics/blob/main/Dashboard%20Screenshots/Dashboard%201.png)

### Dashboard 2: Product Performance Analysis
![Product Performance Analysis dashboard showing units sold, product revenue, category profit, and monthly category trends](https://github.com/Ankar-G/Sales-Performance-Revenue-Growth-Analytics/blob/main/Dashboard%20Screenshots/Dashboard%202.png)

### Dashboard 3: Regional & Sales Representative Performance
![Regional and Sales Representative Performance dashboard showing regional revenue, representative results, target achievement, and monthly regional table](https://github.com/Ankar-G/Sales-Performance-Revenue-Growth-Analytics/blob/main/Dashboard%20Screenshots/Dashboard%203.png)

### Dashboard 4: Customer & Revenue Analysis
![Customer and Revenue Analysis dashboard showing customer segments, top customers, new vs repeat customers, industries, and monthly segment trends](https://github.com/Ankar-G/Sales-Performance-Revenue-Growth-Analytics/blob/main/Dashboard%20Screenshots/Dashboard%204.png)

---

## 20. Connect With Me

> Contact details were not available. Replace the placeholders with the details from your existing portfolio README so this section matches your other projects.

- **Name:** [Ankar Goswami]
- **LinkedIn:** [https://www.linkedin.com/in/ankar-goswami-23a196245/]
- **GitHub:** [https://github.com/Ankar-G]
- **Email:** [goswamijit99@gmail.com]

If you found this project useful, consider giving the repository a star.
