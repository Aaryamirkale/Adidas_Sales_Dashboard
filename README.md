# Adidas US Sales Performance Dashboard — Excel

An end-to-end Excel analytics project built on a 9,648-row Adidas US sales dataset
covering FY 2020–2021 across 10 retailers, 8 products, and 5 regions.

![Dashboard Preview](dashboard_preview.png)

---

## Workbook Structure

| Sheet | Description |
|---|---|
| Executive Dashboard | KPI cards with trend indicators, analyst commentary, and charts |
| Calculations | Core formula layer — SUMIFS, XLOOKUP, COUNTIFS, RANK, MAX/MIN |
| Monthly Trend | Month-by-month 2020 vs 2021 comparison with conditional formatting |
| Pivot Analysis | Region x Category heatmap, Sales Method cross-tab, retailer ranking |
| YoY Analysis | Year-over-year breakdown by Region, Product, Retailer, and Sales Method |
| Raw Data | 9,648 rows structured as a named Excel Table, ready for pivot analysis |

---

## Excel Skills Demonstrated

**Lookup and Reference**
- XLOOKUP — dynamic retailer lookup with fallback handling
- RANK — live retailer revenue ranking that updates with data

**Aggregation**
- SUMIFS — multi-condition sales totals by region, year, and month (181 uses)
- SUMIF — retailer and category-level totals (48 uses)
- AVERAGEIF / AVERAGEIFS — margin analysis by channel and fiscal year
- COUNTIF / COUNTIFS — transaction counts with up to 3 simultaneous conditions

**Statistical**
- MAX / MIN — peak and floor values across months and transactions
- LARGE / SMALL — top-N retailer revenue ranking
- SUMPRODUCT — conditional aggregation across years

**Error Handling**
- IFERROR — suppresses division errors across all ratio calculations (90 uses)
- IF / TEXT — dynamic trend indicators on KPI cards

**Formatting and Visualization**
- Color scale heatmap on Region x Category sales matrix
- Data bars on market share and YoY growth columns
- Red and green conditional formatting on growth percentage rows
- 7 embedded charts across sheets: line, clustered bar, and pie
- Named Excel Table with row striping (AdidasSalesData, 9,649 rows)

---

## Key Findings

- The West region generates the highest revenue, driven by online sales through Amazon and Adidas Direct
- Footwear accounts for over 60% of total revenue, with Men's Athletic Footwear as the top-performing SKU
- Revenue grew approximately 8% year-over-year from 2020 to 2021, with Q4 consistently accounting for around 22% of annual sales
- The online channel carries an average operating margin of 42%, outperforming in-store by 8 to 10 percentage points
- The outlet channel (Kohl's) shows the lowest margin at 31%, representing the clearest opportunity for channel mix improvement

---

## Tools

- Microsoft Excel — formulas, conditional formatting, charts, named tables
- Python with openpyxl and pandas — dataset generation and workbook build

---

## Files

| File | Description |
|---|---|
| Adidas_Sales_Dashboard.xlsx | Main workbook |
| dashboard_preview.png | Screenshot of the Executive Dashboard tab |
