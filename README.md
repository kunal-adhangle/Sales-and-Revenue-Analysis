# Sales and Revenue Analysis Dashboard

## Overview
The Sales and Revenue Analysis Dashboard is designed to provide insights into sales performance, revenue trends, and profitability across different dimensions. This interactive Power BI report enables data-driven decision-making using KPIs, charts, tables, and advanced DAX calculations.

## Dataset Details
The dataset used in this project includes the following fields:
  - Order ID: Unique identifier for each transaction.
  - Date: Transaction date.
  - Customer Name: Name of the customer (some values may be null and handled accordingly).
  - Product: Name of the product sold.
  - Category: Product category classification.
  - Region: Geographical region where the sale occurred.
  - Quantity: Number of units sold.
  - Cost Price: Purchase cost per unit.
  - Selling Price: Sale price per unit.
  - Discount: Discount applied (represented as a decimal percentage).
  - Sales: Total revenue generated per order.
  - Profit: Net profit earned per order.

## DAX Measures Used
Total Sales = SUM(Sales[Sales])

Total Profit = SUM(Sales[Profit])

Profit Margin % = DIVIDE([Total Profit], [Total Sales], 0)

Discount Amount = SUMX(Sales, Sales[Selling Price] * Sales[Discount])

## Interactive Features
  - Cross-filtering enabled: Clicking on a region, category, or product updates all related visuals.
  - Conditional formatting: Highlights significant trends in tables and matrices.
  - Trend analysis: Line charts visualize patterns over time.
  - Edited interactions: Custom interactions applied to the Table Visual for better data exploration.

## Power BI Service Dashboard
<img width="956" alt="Power BI Service Dashboard" src="https://github.com/user-attachments/assets/f1d8f71b-e228-4ba5-b074-60b957c119d2" />

## Power BI Desktop
<img width="953" alt="Power BI Dashboard" src="https://github.com/user-attachments/assets/8c78fa0f-fa67-4a9b-ac95-4cefcc7d64ab" />

