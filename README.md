# Customer Shopping Trends — Exploratory Data Analysis

An exploratory data analysis (EDA) of a 3,900-row retail transactions dataset, examining customer demographics, purchase behavior, and shopping patterns across categories, seasons, payment methods, and customer segments.

## Project Overview

This project walks through a full EDA workflow on a customer shopping dataset:

- **Data quality checks**: confirming the dataset is free of missing values and duplicates
- **Univariate analysis**: distributions of age, gender, category, season, purchase amount, subscription status, and color preferences
- **Bivariate analysis**: relationships between purchase amount, review rating, category, frequency, location, size, payment method, and discounts
- **Multivariate analysis**: a correlation heatmap of numeric features, spend by category × gender, subscription behavior, purchase amount by age group, and revenue by location
- **Key insights**: a summary of the patterns (and notable *lack* of patterns) found across the dataset

## Dataset

**Source:** [Customer Shopping Trends Dataset](https://www.kaggle.com/datasets/iamsouravbanerjee/customer-shopping-trends-dataset) (Kaggle, by Sourav Banerjee)

3,900 records with 19 columns, including:

| Column | Description |
|---|---|
| Customer ID | Unique identifier for each customer |
| Age, Gender | Customer demographics |
| Item Purchased, Category | Product details |
| Purchase Amount (USD) | Transaction value |
| Location, Size, Color, Season | Product/context attributes |
| Review Rating | Customer feedback score |
| Subscription Status | Whether the customer is a subscriber |
| Payment Method, Shipping Type | Transaction logistics |
| Discount Applied, Promo Code Used | Promotional activity |
| Previous Purchases | Customer purchase history |
| Preferred Payment Method | Stated preference |
| Frequency of Purchases | Self-reported shopping cadence |

## Key Findings

- The dataset is clean — no missing values, no duplicate rows.
- Clothing is the most purchased category, but average spend per transaction is nearly identical across all categories, seasons, genders, sizes, age groups, and locations.
- Correlations between the numeric features (Age, Purchase Amount, Review Rating, Previous Purchases) are all close to zero and none of them linearly predict each other.
- Only ~27% of customers are subscribers, and subscribers don't spend more or rate higher than non-subscribers.
- Discounts don't correlate with larger purchase amounts or higher review ratings.

See the notebook for the full breakdown, charts, and discussion of each finding.

## Tools Used

- **Python** — pandas, numpy, matplotlib, seaborn
- **Environment** — Jupyter Notebook

## Files

- `shopping_trends_EDA.ipynb` — the full analysis notebook
- `shopping_trends.csv` — the dataset
- `README.md` — this file

