# Data Cleaning Report

The project uses the cleaned CSV tables provided in the dataset bundle when available. The cleaning workflow removes duplicate records and duplicate primary keys, standardizes city and state text, fills missing ages with the median, labels missing payment methods as `Unknown`, converts date/numeric fields, clips discount percentages to 0–100, removes non-positive quantities and prices, and removes orphaned foreign-key rows.

## Final table sizes
- Customers: 10,000
- Products: 1,000
- Orders: 50,000
- Order items: 102,534

See `tables/data_quality_checks.csv` and `tables/data_validation_checks.csv` for machine-readable checks.
