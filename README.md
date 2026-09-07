# Pizza Sales Dashboard - Executive Review

## Project Overview
This project leverages Business Intelligence to analyze transactional data for "The Pizza Factory," transforming raw sales records into interactive visualizations. The resulting dashboard provides actionable insights to help management optimize inventory, adjust employee schedules, and tailor marketing strategies.

## Dashboard Preview
![Pizza Sales Dashboard](<Images/Screenshot 2026-08-01 232603.png>)

## Data Processing & ETL
The raw dataset, consisting of 48,620 sales records, was imported and cleaned using Power Query in Microsoft Power BI. The transformation workflow included:
* **Data Inspection:** Verified 100% data completeness with no null or blank values across the records.
* **Standardization:** Converted operational columns to proper data types, such as setting the `order_date` to Date and `unit_price` to a Fixed Decimal Number to prevent financial rounding errors.
* **Feature Engineering:** Extracted "Month Name" and "Day Name" from the date field to enable time-series analysis.
* **Financial Metrics:** Engineered a custom `Revenue` column using the formula `[quantity] * [unit_price]` to serve as the primary Key Performance Indicator.

## Key Insights
* **Overall Performance:** The dashboard tracked 16.6K in total revenue across 985 orders, with an average of 1.03 pizzas per order, indicating a strong customer preference for single-item purchases.
* **Sales Trends:** Wednesday and Sunday are the peak business days, generating 2,586 and 2,559 in revenue respectively, while Saturday sees the lowest sales activity.
* **Category & Size Preferences:** The Classic pizza category is the top earner (4.4K), and Large pizzas dominate sales by contributing 46.23% of the total revenue.
* **Top Products:** "The Pepperoni Pizza" and "The Thai Chicken Pizza" are the best-selling menu items, with 59 and 57 total units sold respectively.

## Tech Stack
* **Data Cleaning & Modeling:** Power Query (Microsoft Power BI)
* **Visualization:** Microsoft Power BI
* **Reporting:** PDF Documentation
