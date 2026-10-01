# Retail Executive Dashboard

An interactive **Power BI** dashboard that gives executives a one-page view of retail business performance across **Egyptian cities**, covering **2022 to 2024**: revenue, orders, returns, profit, and progress against targets.

![Dashboard Preview](dashboard-preview.png)

## Highlights

*(Figures shown with the date slicer set to "All")*

| Metric | Value |
|---|---|
| Total Revenue | 45.35M |
| Net Profit | 9.70M |
| Orders Count | 12K |
| Total Returns | 1K |
| Gross Profit Margin | 21% |
| Return Rate | 9% |
| Orders YoY Growth | 51% |
| Average Order Value (AOV) | 3.71K vs. a goal of 3,000 (+23.81%) |

Other things the dashboard shows:

- Quarterly revenue stays above cost in every quarter from 2022 to 2024.
- Most revenue comes from completed orders (about 87%), with the rest split between returned and cancelled orders.
- Revenue is tracked across 9 cities, including Cairo, Alexandria, Giza, Aswan, Luxor, Hurghada, Ismailia, Mansoura, and Port Said.

## Visuals

| Visual | What it shows |
|---|---|
| KPI cards | Revenue, orders, returns, net profit, and their targets and rates |
| KPI visual | AOV by month against the AOV goal |
| Combo chart (line + columns) | Total Revenue vs. Total Cost by quarter and year |
| Donut chart | Stock distribution by product category |
| Donut chart | Revenue split by order status |
| Ribbon chart | Revenue ranking by city across years |
| Waterfall chart | Net Profit change by product category and year |
| Date slicer | Filters the whole page by year, quarter, month, or day |

## Data Model

The report is built on a star schema:

- **Fact tables:** `fact_orders`, `fact_orders_2022_2023`
- **Dimension tables:** `dim_customers`, `dim_products`, `dim_date`

Calculations (Total Revenue, Net Profit, AOV, Return Rate %, YoY Growth %, Gross Profit Margin %, etc.) are written as **DAX measures**.

## How to Open

1. Download `Retail_Dashboard.pbix` from this repository.
2. Open it with [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free, Windows only).
3. Use the date slicer to explore the data.

> GitHub cannot preview `.pbix` files, which is why the screenshot above is included.

## Tools

- Power BI Desktop
- DAX
- Star-schema data modeling

## Author

**zyadbhlol**: [GitHub](https://github.com/zyadbhlol)
