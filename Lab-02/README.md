# Lab 02 — Data Cleaning, Visualization & Interactive Dashboards

**Course:** SRT411 — Digital Data Analytics  
**Submitted:** May 28, 2024  
**Platform:** Microsoft Excel  
**Source:** 23-page academic lab report (PDF to be uploaded separately)

## Overview
This lab builds on Lab 01 by preparing a sales dataset for analysis, selecting and customizing visualizations, creating derived metrics, and building interactive PivotTable-based reports and charts.

## Work documented

### 1. Charting and data storytelling
- Created bar, pie, line, scatter, and stacked-column/bar visualizations for country revenue, product category share, yearly sales, customer age and revenue, and category performance.
- Used **Switch Row/Column**, chart filters, chart-type changes, and formatting to compare alternative analytical views.
- Applied descriptive chart titles, labels, and visual formatting to improve readability.

### 2. Data cleaning and transformation
- Used Excel's **Remove Duplicates** feature; the report documents **1,000 duplicates removed** (113,036 to 112,036 records).
- Standardized country names with `UPPER` and adjusted spacing using `TRIM`.
- Created an age-category feature using `IF`.
- Applied text, number, and custom data filters to isolate values and examine data quality.

### 3. Feature engineering
Created a **Sales Performance Score** using profit, unit price, and unit cost. The report documents the formula:

```excel
=IFERROR((Profit / Unit_Cost) / (Unit_Price / Unit_Cost), 0)
```

### 4. PivotTables, PivotCharts, and dashboard interaction
- Summarized profit and sales by country, age group, product category, product, and month.
- Built charts linked to pivot analyses, including stacked columns, line, pie, bar, and area charts.
- Added **slicers** for Year and Product Category.
- Demonstrated **Refresh All** updating a PivotTable/chart after changing source data; the report shows 2013 Accessories revenue changing from **$3,384,215** to **$3,382,507**.

## Skills demonstrated
**Excel · Data Cleaning · Deduplication · Data Transformation · Feature Engineering · PivotTables · PivotCharts · Data Visualization · Slicers · Interactive Dashboards · Reporting**

## Documentation
The report contains screenshots and explanations for Tasks 01–15. Upload the original PDF into this folder separately, then add a link here.

## Scope
This is an academic Excel analytics lab using sales data, not an independently built security monitoring dashboard or a production analytics system. The original workbook and dataset are not included in this repository.
