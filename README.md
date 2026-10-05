# BrewMetrics BI

A version-controlled Power BI analytics solution for BrewMetrics Coffee Co.
# BrewMetrics BI

## Project Overview

BrewMetrics BI is a Power BI business intelligence project developed
for BrewMetrics Coffee Co. The project analyzes transaction-level
sales data to understand sales performance across different cities,
store formats, categories, products and time periods.

The dashboard provides an interactive way to explore sales trends
and identify differences in product and city performance.

## Technologies

- Power BI Desktop
- GitHub
- GitHub Copilot
- Visual Studio Code
- DAX
- Power Query

## Data Model

The solution follows a star-schema design with a central sales
fact table connected to supporting dimension tables.

### Fact_Sales

Contains transaction-level sales information including date, city,
store format, category, item, quantity, unit price and sales amount.

### Dim_Date

Contains date-related fields used for monthly sales analysis,
filtering and date drill-down.

### Dim_City

Contains city and store-format information used for comparing
sales performance between locations.

### Dim_Product

Contains product and category information used for product-level
and category-level sales analysis.

## DAX Measures

The dashboard includes the following DAX measures:

- Total Sales
- MoM Growth %
- Running Total Sales
- City Sales Rank
- Average Transaction Value

These measures are used in the dashboard KPIs, charts and
interactive analysis.

## Dashboard

The dashboard provides:

- Total Sales KPI
- Month-over-month growth analysis
- Running total sales analysis
- Average transaction value
- Sales trend by month
- City-level sales comparison
- Product-level sales analysis
- Category contribution analysis
- Interactive city, category and item filtering
- Date-based drill-down

## Key Insights

1. Cold Brew sales show a noticeable monthly pattern in the
   available dataset, with sales changing across the April,
   May and June periods.

2. Bengaluru shows stronger overall sales performance compared
   with several of the other cities displayed in the dashboard.

3. The category and product visuals show that sales contribution
   differs between Coffee, Merchandise and Bakery products.

4. The interactive slicers allow users to investigate how sales
   performance changes by city, category and individual product.

## Version Control

The project was developed incrementally using GitHub and GitHub
Desktop.

Separate commits were used to record the major development stages,
including the star schema, individual DAX measures, dashboard
development and project documentation.

The complete commit history is preserved to show the progression
of the project from data modelling through to the final dashboard.

## Project Deliverables

The repository contains:

- Power BI project files
- Source sales data
- README.md
- NOTES.md
- REFLECTION.md
- Final dashboard PDF

## Conclusion

The BrewMetrics BI dashboard provides an interactive view of sales
performance across time, cities, products and categories. The
project demonstrates the use of Power BI, DAX, Power Query,
star-schema modelling, GitHub version control and Copilot-assisted
development in a business intelligence workflow.
