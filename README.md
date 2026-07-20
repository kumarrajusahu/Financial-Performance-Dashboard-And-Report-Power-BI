# Financial Sales & Profitability Analysis — Power BI Dashboard

**Author:** Raju Kumar Sahu
**Tool:** Power BI Desktop
**Dataset:** Financial_Sample.xlsx (700 transactions, 2013–2014)
**Type:** End-to-end multi-page BI dashboard (8 report pages)

---

## Project Overview

This project analyzes two years (2013–2014) of financial sales data across 5 countries, 6 product lines, and 5 customer segments to uncover trends in revenue, profitability, and discounting behavior. The dashboard structured as an 8-page interactive report, moving from a high-level executive summary down to granular, drill-through product-level detail.

The goal was to simulate a real-world business intelligence deliverable — the kind a data analyst would hand to sales, finance, and leadership teams to support quarterly reviews and strategic decisions.

---

## Business Questions Answered

- How are sales and profit trending month-over-month and year-over-year?
- Which countries, segments, and products are the strongest and weakest performers?
- How does discounting affect profit margin across segments?
- Which product-country-segment combinations are most and least profitable?
- What does year-to-date performance look like, and how does it compare to prior year?

---

## Dashboard Structure

| Page | Focus |
|---|---|
| **1. Executive Summary** | Headline KPIs (Total Sales, Gross Sales, Profit, Units Sold, Profit Margin %, Discount %), sales trend by month/year, sales by country and segment |
| **2. Sales Analysis** | Sales breakdown by month & product, by country, and by product mix |
| **3. Profitability Analysis** | Profit by quarter (waterfall view), profit by product/country matrix, gross sales vs. profit by segment |
| **4. Discount Analysis** | Sales and profit by discount band, profit vs. discount % by segment over time |
| **5. Product Performance** | Best/worst performing products, decomposition tree (country → product → segment) |
| **6. Country Analysis** | Sales, profit, margin, and units sold broken down by country |
| **7. Time Intelligence** | YTD sales, YTD profit, YoY growth %, prior-year sales comparison |
| **8. Drill-Through (Product)** | Product-level drill-through page showing monthly and country-level detail for a selected product |

---

## Key Insights

- **Total Sales:** ₹118.73M | **Gross Sales:** ₹127.93M | **Total Profit:** ₹16.89M | **Profit Margin:** 14.23%
- **Government** is the top-performing segment (~44% of sales), followed by **Small Business** (~36%) and **Enterprise** (~17%)
- **Paseo** is the strongest product by both sales and profit; **Velo** has the weakest profit margin despite solid sales volume
- **France and Germany** post the highest profit margins (15.5–15.7%), while the **United States** has the highest sales volume but the lowest margin (~12%) — signaling heavier discounting or a costlier product mix
- Profit **spikes sharply in Q4**, driven largely by October and December
- Sales dipped seasonally around **August**, consistent across both years
- The **Enterprise** segment shows negative profit in at least one product/region combination, flagging it for margin review

---

## Approach & Methodology

1. **Data validation** — Cross-checked totals (sales, profit, units sold) across pages to ensure consistency after aggregations and filters.
2. **KPI design** — Selected headline metrics (Sales, Profit, Margin %, Discount %) that map directly to how sales/finance teams review performance.
3. **Visual layout** — Structured the report as a narrative: summary → detailed sales → profitability → discounting → product/country deep dives → time trends → drill-through, so a reader can go as broad or as deep as needed.
4. **Time intelligence** — Built YTD and YoY growth measures to support period-over-period comparison, a standard requirement in financial reporting.
5. **Interactivity** — Added slicers (Year/Month), a decomposition tree, and a drill-through page so stakeholders can self-serve deeper cuts of the data without needing a new report built for them.

---

## Tools & Skills Demonstrated

- Power BI Desktop (data modeling, DAX measures, report design)
- DAX for Time Intelligence (YTD, YoY Growth %, Prior Year comparisons)
- Data visualization design (KPI cards, waterfall charts, scatter plots, decomposition tree, treemap, drill-through)
- Business-oriented KPI selection and dashboard storytelling
- Data validation and cross-checking across report pages

---

## Files

- `Financial_Sample.xlsx` — source dataset
- `Financial_analysis.pbix` — Power BI project file
- `Financial_analysis.pdf` — exported dashboard (all 8 pages)

---

## Future Improvements

- Add profitability forecasting using historical trend lines
- Build a discount-optimization view to flag segments where discounting is eroding margin without driving proportional volume
- Add row-level security to simulate country-manager-specific dashboard views
