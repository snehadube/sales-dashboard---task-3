# Simple Sales Dashboard — Sample Superstore

## Objective
Turn cleaned Sample Superstore data and KPIs into an interactive dashboard that a
stakeholder could actually use — showing sales performance by **Product Category**,
**Region**, **Segment**, and **Month**.

## Tool used
**Microsoft Excel** (`.xlsx`). Built with `openpyxl` + formulas, verified in LibreOffice —
no external BI license required to open it.

## What's inside (`Sales_Performance_Dashboard.xlsx`)
| Sheet | Purpose |
|---|---|
| **Dashboard** | The main view: 2 filters, 4 KPI cards, 3 charts |
| **How to Read This Dashboard** | One-page note explaining how to use it |
| **Calc** | SUMIFS helper tables that feed the charts (kept transparent, not hidden) |
| **Data** | Full cleaned dataset (9,994 rows, 21 columns) as supplied |

## Interactivity (the slicer/filter requirement)
Two dropdown filters on the Dashboard sheet — **Region** and **Year** — drive every KPI
card and all three charts live via `SUMIFS` formulas (no hardcoded numbers, no VBA).

## KPIs (kept to 4, per the "3-4 KPIs max" guidance)
- Total Sales
- Total Profit
- Units Sold
- Profit Margin %

## Visuals (3, minimum met)
1. **Sales by Category** — column chart (Furniture / Office Supplies / Technology)
2. **Sales by Segment** — pie chart (Consumer / Corporate / Home Office)
3. **Monthly Sales Trend** — line chart (Jan–Dec), useful for spotting seasonality

## Dataset
[Sample Superstore Dataset](Sample_Superstore_Cleaned_UTF8.csv) — cleaned version
(duplicates removed on `order_id`), originally sourced from Kaggle. See
`Samplesuperstore_analysis.sql` for the MySQL cleaning/EDA queries this dashboard builds on.

## How to open
1. Download `Sales_Performance_Dashboard.xlsx`
2. Open in Excel
3. Use the **Region** and **Year** dropdowns on the Dashboard tab to filter

## Repo contents
- `Sales_Performance_Dashboard.xlsx` — the dashboard deliverable
- `Sample_Superstore_Cleaned_UTF8.csv` — source data
- `Samplesuperstore_analysis.sql` — SQL cleaning/analysis behind the dataset
