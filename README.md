📊 Customer Shopping Behavior Analysis
End-to-End Data Analysis Project (Python, SQL, Power BI)
📝 1. Project Overview

This project analyzes customer shopping behavior using transactional data from 3,900 purchases across multiple product categories.
The goal is to uncover insights into:

Spending patterns

Customer segmentation

Product popularity

Subscription behavior

Factors influencing purchase decisions

These insights help businesses improve targeting, marketing, pricing, and customer retention.

📂 2. Dataset Summary

Rows: 3,900

Columns: 18

Key Features:

Customer demographics: age, gender, location, subscription status

Purchase details: item, category, amount, size, color, season

Behavior: discount applied, previous purchases, frequency, review rating

Shipping type information

Missing Data: Only in the review_rating column (37 nulls)

🐍 3. Exploratory Data Analysis (Python)

Key Python tasks performed:

✔️ Data Preparation

Loaded data using pandas

Examined structure with .info() and .describe()

Checked null values and handled missing ratings using median imputation by product category

✔️ Data Cleaning

Standardized column names to snake_case

Removed redundant columns (promo_code_used dropped after correlation check)

✔️ Feature Engineering

Created age_group based on age bins

Created purchase_frequency_days

Ensured consistency between discount-related features

✔️ Database Integration

Connected to PostgreSQL

Loaded the cleaned DataFrame into SQL for deeper analytical queries

🗄️ 4. SQL Analysis (PostgreSQL)

Business-focused queries were run to extract insights:

Revenue by Gender – Compared total spending

High-Spending Discount Users – Customers who used discounts but still spent above average

Top 5 Products by Rating

Shipping Type Comparison – Standard vs Express average spend

Subscribers vs Non-Subscribers – Revenue & average purchase comparison

Discount-Dependent Products – Products most purchased using discounts

Customer Segmentation – New vs Returning vs Loyal customers

Top 3 Products per Category

Repeat Buyers & Subscriptions – Relationship between high purchase count and subscription rate

Revenue by Age Group

📊 5. Dashboard (Power BI)

A fully interactive Power BI dashboard was created featuring:

Total revenue insights

Product category performance

Customer segmentation visualization

Subscription revenue comparison

Shipping type analysis

Ratings and discount behavior

💡 6. Business Recommendations

Based on the insights, these strategies are suggested:

Boost Subscription Program through exclusive offers

Loyalty Rewards for repeat buyers

Optimize Discount Strategy to balance sales and margins

Highlight Top-Rated Products in marketing campaigns

Target High-Revenue Age Groups

Promote Express Shipping to high-value customers

