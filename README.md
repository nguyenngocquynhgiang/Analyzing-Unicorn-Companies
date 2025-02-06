# Analyze International Debt Statistics

## Project Overview

In the [**Analyze International Debt Statistics**](https://shard-particle-6f4.notion.site/Analyze-International-Debt-Statistics-1772d939cc0c8071be63f28bb1f0abf7?pvs=4) project, I will analyze international debt data from the World Bank using SQL queries. SQL is an essential tool for efficient data analysis.

### Objectives
- Write SQL queries to answer interesting questions about international debt using data from The World Bank.
- Gain insights into country-specific and global debt trends.
- Apply SQL skills to a real-world dataset.

### Key Tasks
1. Identifying distinct countries.
2. Listing distinct debt indicators.
3. Calculating the total amount of debt owed by each country.
4. Finding the country with the highest debt.
5. Computing the average amount of debt across indicators.
6. Identifying the highest amount of principal repayments.
7. Finding the most common debt indicator.

### Additional Learning
I will connect to the [**World Nations**](https://www.datacamp.com/workspace/datasets/sample-integration-mariadb) MariaDB dataset and apply similar queries to gain more experience in SQL database analysis. Additionally, I will take the [**Exploratory Data Analysis in SQL**](https://www.datacamp.com/courses/exploratory-data-analysis-in-sql) course to learn advanced techniques for working with various SQL databases.

## Project Description

In this project, I will analyze international debt data collected by The World Bank. The dataset shows the amount of debt (in USD) that developing countries owe across various categories. I will use data manipulation skills to determine which countries have the highest and lowest debt amounts and create a summary report.

## 1. Exploring the Dataset

| Column | Definition | Data Type |
| --- | --- | --- |
| country_name | Name of the country | varchar |
| country_code | Code representing the country | varchar |
| indicator_name | Debt indicator description | varchar |
| indicator_code | Code representing the debt indicator | varchar |
| debt | Value of the debt indicator (in current US dollars) | float |

### Dataset Insights
- The dataset contains 124 countries.
- Includes multiple indicators related to external debt, principal repayments, and disbursements.
- Provides a broad view of global debt trends.

## 2. Analysis

### 2.1 Country with the Highest Amount of Debt
Using SQL aggregation functions, I found that **China** has the highest total debt, approximately **285.79 billion USD**.

### 2.2 Country with the Lowest Amount of Principal Repayments
Timor-Leste has the lowest amount of principal repayments for external long-term debt, with a repayment amount of **825,000 USD**.

### 2.3 Top 5 Countries with the Highest Total Debt
The top 5 countries with the highest total debt:
1. **China** - 285.79 billion USD
2. **Brazil** - 280.62 billion USD
3. **South Asia Region** (aggregate)
4. **Russia**
5. **Least Developed Countries (UN Classification)**

### 2.4 Total Debt by Each Indicator
The most significant debt category is **"Principal repayments on external debt, long-term (AMT, current US$)"**, contributing **732.20 billion USD**.

### 2.5 Average Debt per Country
- China has the highest average debt per record (~11.91 billion USD).
- Brazil follows closely at **11.69 billion USD**.

### 2.6 Exploring Outliers
Outliers were identified using SQL queries filtering values exceeding two standard deviations above the mean.
- **China and Brazil** had multiple outliers, reinforcing their significant debt burden.
- **Long-term debt repayments** were a primary source of high debt values.

## 3. Summary Report

**Key Findings:**
- China and Brazil dominate in total debt owed.
- Certain economic regions, like South Asia and Least Developed Countries (UN Classification), also report high aggregated debt.
- Principal repayments on external long-term debt contribute the most to total debt.
- Debt distribution varies significantly across countries and regions, with notable outliers.

**Future Work:**
- Further analysis on debt trends over time.
- Examining debt sustainability and repayment capacity.
- Applying machine learning techniques to predict debt growth and default probabilities.

This project serves as a solid foundation for deeper insights into global debt statistics using SQL.

