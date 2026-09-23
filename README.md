# Sales & Customer Performance Dashboard

A Power BI dashboard analyzing retail sales performance across time, region, and product category — built on a 1,000,000+ row transaction dataset.

## Data Model
Star schema:
- `fact_table` — 1,000,000+ transaction line items
- `customer_dim` — 9,191 customers
- `store_dim` — 726 stores (division / district / upazila)
- `time_dim` — calendar dimension (date, month, quarter, year)

## DAX Measures
- `TOTAL SALES`, `TOTAL QTY`, `AVG UNIT PRICE`
- `ACTIVE CUSTOMERS`, `RETURNING CUSTOMERS %`, `MONTHLY NEW CUSTOMERS`
- `% YOY SALES`, `% YOY QTY`, `% YOY CUSTOMER`, `% YOY AVG PRICE`

## Report Pages
1. **Year-wise Analysis** — total sales/quantity trends, YoY growth, monthly patterns, location-wise sales map
2. **Customer and Product Insight** — active customers by order bucket, new-customer trends, product performance, location-wise sales (ribbon chart)

## Key Findings
Verified directly against the source data:
- The **Dhaka** division alone drove **~39% of total sales** — more than double the next-highest region (Chittagong)
- **Food** and **Beverage** categories together contributed **~65% of total revenue**
- Sales were stable year-over-year from 2014–2020, with growth never exceeding ±5.3%

A deeper SQL-based analysis of the same dataset (window functions, CTEs, customer segmentation) is available in a separate repo — see my GitHub profile for the `ecommerce-sql-analysis` project.

## Dataset
Retail transaction dataset provided during the AICTE TechSaksham AI internship, used to practice Power BI data modeling, DAX, and time-intelligence calculations.

## Tech
Power BI Desktop · DAX · Star Schema Data Modeling
