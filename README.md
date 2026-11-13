# Retail Sales & Business Performance Analysis

An end-to-end retail sales analysis project built with **Microsoft Excel**. The project demonstrates data preparation, validation, business analysis, and an interactive dashboard designed to communicate performance trends and operational findings.

## Project overview

The workbook contains 12,000 transaction records across 2024–2025 and 23 fields covering orders, customers, products, sales, costs, profit, payment methods, order status, delivery days, and SLA status.

The analysis focuses on:
- Sales and profit performance over time
- Regional and category contribution
- Product and customer-segment performance
- Payment-mode and order-status patterns
- Delivery SLA performance
- Interactive exploration using Region and Year slicers

## Tools and Excel features

- Microsoft Excel 2019
- Power Query for data cleaning and transformation
- PivotTables for business analysis
- PivotCharts for visual reporting
- Slicers for interactive Region and Year filtering
- Excel formulas for KPI calculations and data validation

## Data preparation and quality checks

The original raw-data worksheet was preserved. A separate cleaned-data worksheet was prepared.

Key preparation steps:
1. Removed 12 exact duplicate records, leaving 12,000 transaction records.
2. Replaced missing Customer Segment and City values with `Unknown` to retain records without inventing classifications.
3. Recovered 20 missing Discount values using the relationship between Sales, Quantity, and Unit Price.
4. Validated Sales against Quantity × Unit Price × (1 − Discount), allowing a ₹0.01 rounding tolerance.
5. Validated Total Cost, Profit, delivery dates, and Delivery Days against their corresponding calculations.
6. Removed temporary validation/helper columns after checks were complete.

## Key findings

### Overall performance

| KPI | Result |
|---|---:|
| Total Sales | ₹770.19M |
| Total Profit | ₹152.38M |
| Total Orders | 12,000 |
| Overall Profit Margin | 19.78% |

### Year-over-year performance

| Measure | 2024 | 2025 | Change |
|---|---:|---:|---:|
| Sales | ₹382.91M | ₹387.28M | +1.14% |
| Profit | ₹76.11M | ₹76.27M | +0.20% |
| Profit Margin | 19.88% | 19.69% | -0.19 percentage points |

Sales increased in 2025, while profit grew more slowly and the overall margin declined slightly. This indicates pressure on profitability; further cost, discount, and product-mix analysis would be needed to identify causes.

### Regional performance

- South contributed the highest share of revenue at 34.32%.
- East contributed the lowest share at 16.97%.
- South and West together contributed 60.67% of total revenue.

### Category and product performance

- Accessories had the highest category profit margin at 35.52%.
- Laptop had the lowest category profit margin at 17.32%.
- Gaming Laptop generated the highest product revenue (₹216.73M) and profit (₹34.17M), with a 15.77% margin.
- Optical Mouse recorded the highest product profit margin at 53.72%.

### Delivery SLA

The dashboard shows 57% of orders within SLA and 43% delayed. The delayed share is an operational area worth investigating; this analysis does not establish the cause of delays.

## Dashboard

The dashboard includes:
- KPI cards for Sales, Profit, Orders, and Profit Margin
- Monthly Sales & Profit Trend
- Regional Sales
- Category Sales
- Delivery SLA Compliance
- Region and Year slicers that filter the dashboard
- A written business-insights section

## Repository files

The repository is intended to contain:

- `Retail_Sales_Business_Performance_Dashboard.xlsx` — interactive Excel workbook with raw data, cleaned data, PivotTables, charts, and dashboard.
- `Retail_Sales_Business_Performance_Dashboard.pdf` — printable dashboard export.
- `Screenshots/Dashboard.png` — dashboard preview image.

## How to explore

1. Download and open the Excel workbook in Microsoft Excel.
2. Open the Dashboard worksheet.
3. Use the Region and Year slicers to filter the KPIs and charts.
4. Review the supporting PivotTable worksheets for the underlying analysis.
5. Open the PDF for a static, print-friendly view.

## Notes and limitations

- The written business insights summarize overall project findings; they are not dynamically rewritten when slicers change.
- The dashboard KPIs and charts respond to the Region and Year slicers.
- Findings describe patterns in this dataset and should not be interpreted as proof of causation.

## Author

**Kamalesh S**

