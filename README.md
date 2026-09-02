# E-Commerce SQL Analysis

SQL analysis project built on the [UK Online Retail dataset](https://www.kaggle.com/datasets/carrie1/ecommerce-data), practicing and applying core to advanced SQL concepts using MotherDuck (DuckDB).

## Dataset
Transaction-level data from a UK-based online retailer, containing:
- `InvoiceNo` — order/invoice ID
- `StockCode` — product code
- `Description` — product name
- `Quantity` — units purchased
- `InvoiceDate` — date and time of purchase
- `UnitPrice` — price per unit
- `CustomerID` — unique customer ID
- `Country` — customer's country

## Business Insights

- UK is by far the biggest market by orders and revenue, with other countries contributing much smaller shares.
- A small group of customers order 200+ times — likely wholesale/resellers rather than regular shoppers, worth treating differently (bulk pricing, dedicated support).
- A large share of customers only order once — the biggest opportunity here is second-order conversion.
- "Top product" changes depending on whether you measure by quantity sold or revenue earned — both are worth tracking.
- Some countries have no single dominant product — demand is spread across several items rather than driven by one bestseller.
- Thursday is consistently the busiest order day — useful for planning promotions and stock readiness.
- Revenue shows clear month-to-month seasonality — useful for advance inventory and staffing planning.

## Tools

- [MotherDuck](https://motherduck.com/) (cloud DuckDB) for running the SQL
- Dataset sourced from Kaggle
