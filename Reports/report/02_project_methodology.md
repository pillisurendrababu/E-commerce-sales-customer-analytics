# Project Methodology

1. Load customer, product, order and order-item CSV files.
2. Inspect table dimensions, data types, duplicates and missing values.
3. Clean duplicate keys, normalize city/state labels, handle missing age and payment method values, and remove invalid quantities.
4. Validate primary-key uniqueness and foreign-key relationships.
5. Join transactional tables to calculate line-level sales, discount, cost and profit.
6. Filter delivered orders for the main commercial KPI analysis.
7. Aggregate performance by month, category, product, customer, state, city, payment method, gender and age group.
8. Calculate customer recency, frequency and monetary value, then assign illustrative RFM segments.
9. Export CSV tables and charts for dashboard development.

## Metric definitions
- Gross sales = quantity × unit price.
- Discount amount = gross sales × discount percentage.
- Net revenue = gross sales − discount amount.
- Cost = quantity × product cost price.
- Profit = net revenue − cost.
- Profit margin = total profit ÷ total net revenue × 100.
- Average order value = delivered revenue ÷ distinct delivered orders.

Discount is applied once to each order's item-line totals by multiplying each line's gross sales by the order discount rate.
