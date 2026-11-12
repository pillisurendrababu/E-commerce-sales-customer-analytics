# E-Commerce Sales & Customer Analytics

An end-to-end data analytics portfolio project using a realistic **synthetic Indian e-commerce dataset** to examine sales performance, product profitability, customer behaviour, and geographic patterns.

The project follows a complete analytics workflow:

**Raw Data → Data Cleaning → Data Validation → MySQL → SQL Analysis → Python EDA → Power BI Dashboard → Business Insights**

The goal is to transform raw transactional data into meaningful insights that can support sales, marketing, customer-retention, and business decision-making.

> **Important dataset note:** The dataset is synthetic. The reported KPIs and findings describe this generated dataset only; they are not actual results from a real e-commerce company or representative estimates of the Indian e-commerce market.

---

## 1. Business Problem

E-commerce businesses generate data across customers, products, orders, payments, and order items. Without structured analysis, it can be difficult to understand what drives revenue, which products are profitable, how customers behave, and where sales are strongest.

This project uses transactional data to answer practical business questions, including:

- Which product categories and products contribute most to revenue and profit?
- How do sales change over time?
- Which states generate the highest revenue?
- Which payment methods are most commonly associated with revenue?
- How frequently do customers purchase?
- Which customer segments may need retention campaigns?
- How do customer demographics relate to purchasing patterns?

## 2. Business Objectives

- Analyze overall sales revenue and profitability.
- Identify high-performing product categories and products.
- Analyze monthly revenue trends.
- Identify top-performing states and geographic markets.
- Understand customer purchasing behaviour.
- Analyze customer purchase frequency and segmentation.
- Evaluate payment-method performance.
- Identify important customer and product insights.
- Build an interactive Power BI dashboard for business reporting.

## 3. Dataset

The project uses a realistic synthetic dataset representing an Indian online retail business.

### Dataset tables

| Table | Description |
|---|---|
| Customers | Customer information such as age, gender, city, and state |
| Products | Product, category, brand, cost price, and selling price |
| Orders | Order dates, customers, payment methods, discounts, and order status |
| Order Items | Products purchased, quantities, and unit prices |

### Dataset size

| Dataset | Records |
|---|---:|
| Customers | 10,000 |
| Products | 1,000 |
| Orders | 50,000 |
| Order Items | 102,559 |

The raw dataset intentionally includes data-quality issues so the project can demonstrate a realistic cleaning and validation workflow.

## 4. Data Cleaning & Validation

Python and Pandas were used to investigate and clean the raw datasets.

### Data-quality issues identified

- Duplicate customer records
- Missing customer ages
- Missing payment methods
- Inconsistent city capitalization
- Invalid order-item quantities
- Data relationship and integrity issues

### Cleaning actions

- Removed exact duplicate customer records.
- Filled missing customer ages using the median age.
- Standardised city names.
- Replaced missing payment methods with `Unknown`.
- Removed order-item records with invalid quantities.
- Converted dates and numeric fields to appropriate data types.
- Rechecked relationships between customers, orders, products, and order items.

The project reports that its critical validation checks passed after cleaning.

## 5. Tools & Technologies

- **Python** – data inspection, cleaning, validation, and analysis
- **Pandas** – data manipulation
- **NumPy** – numerical operations
- **Matplotlib & Seaborn** – data visualisation
- **MySQL** – relational data storage and querying
- **MySQL Workbench** – database management
- **SQL** – business and customer analytics
- **Power BI** – interactive dashboards
- **Microsoft Excel** – data inspection and validation
- **VS Code** – development environment
- **Git & GitHub** – version control and project documentation

## 6. Python Analysis

Python was used for:

- Data inspection and quality analysis
- Data cleaning and validation
- Exploratory Data Analysis (EDA)
- Customer analysis
- Product and category analysis
- Sales and profitability analysis
- Customer segmentation
- Discount analysis
- Business-insight generation

The analysis covers revenue, profit, product performance, category performance, customer behaviour, payment methods, age groups, gender, geography, and purchasing frequency.

## 7. SQL Analysis

MySQL was used to store and analyse the cleaned datasets.

SQL analysis includes:

- Overall business KPIs
- Revenue and profit analysis
- Monthly sales trends
- Category and product performance
- Customer analysis
- State-level analysis
- Payment-method analysis
- Customer segmentation
- RFM analysis
- Window functions and product ranking
- Analytical SQL views

Techniques include joins, aggregations, conditional logic, and advanced analytical queries.

## 8. Power BI Dashboard

The Power BI dashboard contains **three pages**, each designed around a different set of business questions.

### Page 1: Sales Overview

Provides a high-level view of business performance.

Key visuals:
- Total Revenue
- Total Profit
- Profit Margin
- Delivered Orders
- Average Order Value
- Monthly Revenue Trend
- Revenue by Category
- Profit by Category

### Page 2: Product & Customer Performance

Focuses on top-performing products and customers.

Key visuals:
- Top 10 Products by Revenue
- Top 10 Customers by Revenue
- Top 10 Products by Profit
- Revenue by Payment Method
- Customer Segmentation

### Page 3: Customer & Geographic Insights

Focuses on customer demographics, purchasing behaviour, and geographic performance.

Key visuals:
- Revenue by State
- Revenue by Gender
- Revenue by Age Group
- Customer Purchase Frequency

## 9. Key Business Results

The following results are reported for **delivered orders in the synthetic dataset**:

| KPI | Result |
|---|---:|
| Total Revenue | ₹78.47 Cr |
| Total Profit | ₹23.45 Cr |
| Profit Margin | 29.88% |
| Delivered Orders | 28,683 |
| Average Order Value | ₹27,357.58 |

### Category insights

- **Electronics** generated the highest revenue and profit among the product categories.
- Home & Kitchen and Sports followed Electronics in revenue.

### Geographic insights

- **Gujarat** was the highest-revenue state, followed by Kerala and Telangana.

### Payment insights

- **UPI** generated the highest revenue among the available payment methods in this dataset.

### Customer insights

RFM analysis grouped customers into segments including:
- Champions
- Loyal Customers
- Potential Loyalists
- At Risk
- Lost Customers
- Others

The analysis also identified differences in purchasing frequency and customer value across segments.

### Customer demographics

- The **36–45 age group** generated the highest revenue among the age groups analysed.

> These are dataset-specific findings, not verified market-wide trends. Recalculate and cross-check the figures against the final scripts, SQL outputs, and Power BI model before using them in a presentation or resume.

## 10. Business Recommendations

Based on the reported analysis of the synthetic dataset:

1. **Prioritise strong product categories**
   - Electronics is the leading revenue and profit category in this dataset. Inventory and promotional planning could prioritise its high-performing products.

2. **Strengthen high-value customer retention**
   - Champions and loyal customers could be considered for targeted loyalty offers and relevant promotions.

3. **Re-engage at-risk customers**
   - At-risk segments could be evaluated for retention campaigns, personalised offers, and targeted communication.

4. **Review the digital payment experience**
   - UPI generated the highest revenue in this dataset. The business could examine the payment journey and evaluate opportunities to improve convenience.

5. **Use regional performance to guide planning**
   - Gujarat, Kerala, and Telangana were the top states by revenue in this dataset. Regional marketing and inventory plans could take these results into account.

6. **Understand high-revenue customer groups**
   - The 36–45 age group contributed the most revenue in this dataset. Further analysis could examine its product preferences and purchasing frequency before designing targeted campaigns.

Recommendations are hypotheses for business action based on the dataset; their real-world impact would need to be tested.

## 11. Project Workflow

1. Inspect the raw datasets and understand their fields.
2. Identify missing values, duplicates, invalid records, and inconsistent formats.
3. Clean and validate the data while retaining the raw source files.
4. Load the cleaned data into MySQL.
5. Write SQL queries to answer business questions.
6. Perform exploratory analysis and visualisation in Python.
7. Build a Power BI dashboard around relevant KPIs.
8. Summarise findings and develop evidence-based business recommendations.

## 12. Repository Structure

```text
e-commerce-sales-customer-analytics/
│
├── data/
│   ├── raw/
│   └── cleaned/
│
├── python/
│   ├── 01_data_inspection.py
│   ├── 01_eda.py
│   ├── 02_business_analysis.py
│   ├── 02_data_quality.py
│   ├── 03_data_cleaning.py
│   ├── 04_data_validation.py
│   ├── 05_mysql_connection_test.py
│   ├── 06_load_data_to_mysql.py
│   ├── 07_eda.py
│   ├── 08_discount_analysis.py
│   ├── 09_final_business_insights.py
│   └── generate_dataset.py
│
├── sql/
│   ├── 01_create_tables.sql
│   ├── 01_basic_business_analysis.sql
│   ├── 02_sales_analysis.sql
│   └── 03_advanced_analysis.sql
│
├── powerbi/
│   └── E-Commerce_Sales_Customer_Analytics.pbix
│
├── reports/
│   ├── business_insights.md
│   └── charts/
│
└── README.md
```

Update this structure if the actual repository uses different file or folder names.

## 13. Project Outcomes

This project demonstrates an end-to-end data analytics workflow, from raw-data inspection and cleaning to SQL analysis, Python EDA, dashboard reporting, and business recommendations.

It is designed to showcase practical skills relevant to Data Analyst, Business Analyst, Business Operations Analyst, and BI Analyst roles.

---

## Author

**PILLI SURENDRA BABU**


