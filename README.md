# pandas-challenge-1
Module 4 Challenge - Ken Stager

# Module 4 Data Analysis Project

## Overview

This project is a part of the Module 4 Challenge in the Columbia University AI Bootcamp, focusing on data analysis using Python and the Pandas library. The aim is to explore, transform, verify, and summarize a dataset from a fictional e-commerce company to derive actionable financial insights.

## Key Objectives

- **Data Exploration**: Familiarize with the dataset through basic statistical summaries and identification of key categories.
- **Data Transformation**: Enhance the dataset by calculating additional financial metrics such as subtotal, shipping price, total price, cost, and profit for each order.
- **Data Verification**: Validate the accuracy of the calculated data against provided totals for specific orders.
- **Data Summary and Analysis**: Create a summary DataFrame for top clients, showcasing their total units purchased, shipping price, revenue, and profit.

## Dataset Overview

The dataset comprises client orders from an e-commerce platform, including columns like `client_id`, `order_id`, `item_category`, `unit_price`, `qty`, and more.

## Data Exploration

Initial exploration involved viewing the first few rows of the dataset using `df.head()` and examining basic statistics with `df.describe(include="all")`. This step was crucial for understanding the dataset's structure and basic characteristics.

## Data Transformation

Key transformations included:

- Calculating the `subtotal` for each line item based on `unit_price` and `qty`.
- Deriving the `shipping_price` based on item weight, with different rates for orders above and below 50 pounds.
- Adding a `total_price` column factoring in the subtotal, shipping price, and a sales tax of 9.25%.
- Computing the `line_cost` and `line_profit` for each order line.

## Data Verification

The calculated totals for specific orders were verified against provided totals to ensure the accuracy of our data transformations. This verification step confirmed the reliability of the subsequent analysis.

## Key Insights

- Identified the top three item categories with the most entries.
- Analyzed the most popular subcategory within the top item category.
- Listed the top five clients based on the number of orders.
- Determined the total units ordered by the top client.

## Summary and Analysis

A summary DataFrame was created for the top five clients, which included:

- Total units purchased.
- Total shipping cost.
- Total revenue.
- Total profit.

This data was further formatted for presentation, converting currency values to millions of dollars and renaming columns for clarity.

## Conclusion

This project demonstrates the practical application of Python and Pandas in data analysis, from initial exploration to deriving actionable insights, particularly focusing on customer behavior and profitability.

## Future Work

Future enhancements could include deeper analysis into seasonal trends, product performance, and client purchasing patterns to further inform business strategies.

