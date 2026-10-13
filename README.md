# Supermarket Sales Analysis Dashboard | Power BI

An interactive Power BI dashboard designed to explore supermarket sales performance, profitability, product performance, category contribution, and monthly trends.

## Dashboard Preview

![Supermarket Sales Dashboard](screenshots/dashboard.png)

## Project Overview

This beginner-friendly data analytics project uses a sample supermarket sales dataset with 150 orders. It brings key business metrics together in a single interactive report.

## Tools and Skills

- Microsoft Power BI Desktop
- DAX measures
- Data visualization and report design
- Interactive slicers and filter context
- Sales performance analysis

## Dashboard Features

- KPI cards: Total Sales, Total Profit, Profit Margin, Total Orders, Average Order Value
- Sales by Product bar chart
- Sales by Category donut chart
- Monthly Sales Trend line chart
- City dropdown slicer for interactive filtering

## DAX Measures

```dax
Total Sales = SUM(supermarket_sales[Sales])
Total Profit = SUM(supermarket_sales[Profit])
Profit Margin % = DIVIDE([Total Profit], [Total Sales], 0)
Total Orders = DISTINCTCOUNT(supermarket_sales[Order ID])
Average Order Value = DIVIDE([Total Sales], [Total Orders], 0)
```

## Dashboard Results

Values below are approximate, as displayed in the unfiltered dashboard screenshot:

| Metric | Value |
| --- | ---: |
| Total Sales | 356K |
| Total Profit | 96K |
| Profit Margin | 26.88% |
| Total Orders | 150 |
| Average Order Value | 2.37K |

### Key Insights

- Coffee is the highest-revenue product.
- Beverages contribute the largest share of category sales (approximately 62.74%).
- July records the highest monthly sales in the displayed January–September period.

## Repository Structure

```text
Supermarket-Sales-PowerBI-Dashboard/
├── README.md
├── Supermarket_Sales_Dashboard.pbix
├── supermarket_sales.csv
└── screenshots/
    └── dashboard.png
```

## How to View the Project

1. Download the `.pbix` file from this repository.
2. Open it in Microsoft Power BI Desktop.
3. Explore the KPIs and charts and use the City slicer to filter the results.

> **Note:** This project is based on a sample dataset for learning and portfolio demonstration. Values are illustrative, not real business results.

## Author

Ravindu Alwis — Data Science Undergraduate, SLIIT
