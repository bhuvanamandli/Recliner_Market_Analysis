# Recliner Market Analysis

## Overview

This project focuses on analyzing recliner products available on the Pepperfry platform using Web Scraping, Data Preprocessing, Exploratory Data Analysis (EDA), Data Visualization, Feature Engineering, and Hypothesis Testing.

The objective of this project is to understand recliner pricing patterns, brand-wise trends, customer preferences, discount strategies, warranty offerings, and other factors that influence recliner prices. The analysis helps identify value-for-money products and provides meaningful business insights from real-world e-commerce data.

---

## Business Problem

Customers often face difficulty while purchasing recliners online because:

* A large number of recliner options are available.
* Similar recliners have significant price differences.
* Discounts and EMI offers create confusion.
* Buyers find it difficult to identify value-for-money products.

Furniture companies can also benefit from understanding:

* Pricing strategies
* Customer preferences
* Market trends
* Product positioning

---

## Project Objectives

* Extract recliner data from Pepperfry using Selenium Web Scraping.
* Perform data preprocessing and feature engineering.
* Analyze pricing, discounts, and market trends.
* Identify factors affecting recliner prices.
* Generate insights using EDA and hypothesis testing.
* Help customers make data-driven buying decisions.

---

## Dataset Information

The dataset was collected from Pepperfry using Selenium Web Scraping.

### Features

| Column Name      | Description               |
| ---------------- | ------------------------- |
| Brand            | Recliner brand name       |
| Model            | Recliner model            |
| Color            | Product color             |
| Seater           | Seating capacity          |
| Rating           | Customer rating           |
| Warranty(Months) | Warranty period in months |
| Original Cost    | Original listed price     |
| Discount(%)      | Discount percentage       |
| Final Price      | Price after discount      |
| EMI              | Monthly EMI amount        |
| Shipping Days    | Estimated delivery time   |

---

## Technologies Used

* Python
* Selenium
* Pandas
* NumPy
* Matplotlib
* Seaborn
* SciPy
* Jupyter Notebook

---

## Project Workflow

Business Understanding

↓

Web Scraping using Selenium

↓

Dataset Creation

↓

Data Cleaning & Preprocessing

↓

Feature Engineering

↓

Exploratory Data Analysis (EDA)

↓

Data Visualization

↓

Hypothesis Testing

↓

Business Insights & Recommendations

---

## Data Preprocessing

The following preprocessing steps were performed:

### Data Cleaning

* Removed unnecessary columns.
* Checked dataset structure and summary statistics.
* Verified data types.

### Missing Value Handling

* Filled missing categorical values using mode.
* Filled missing numerical values using median.

### Duplicate Handling

* Identified and removed duplicate records.

### Data Type Conversion

* Converted columns into appropriate data types.

### Outlier Analysis

* Applied Z-Score method.
* Applied IQR method.
* Validated outliers using domain knowledge before removal.

---

## Feature Engineering

Additional features were created to improve analysis:

### Discount Amount

Discount Amount = Original Cost - Final Price

### Warranty Years

Warranty(Years) = Warranty(Months) / 12

### Price Category

Recliners were categorized into:

* Budget (0–30000)
* Mid-Range (30001–70000)
* Premium (70001–150000)
* Luxury (150001–300000)

---

## Exploratory Data Analysis

### Univariate Analysis

Numerical Variables

* Histogram with KDE
* Boxplots

Categorical Variables

* Brand Distribution
* Color Distribution

### Bivariate Analysis

Numerical vs Numerical

* Final Price vs Rating
* Final Price vs EMI
* Final Price vs Warranty
* Correlation Heatmap

Categorical vs Numerical

* Brand vs Final Price
* Seater vs Final Price

Categorical vs Categorical

* Brand vs Color
* Brand vs Price Category
* Seater vs Price Category

### Multivariate Analysis

* Pair Plot Analysis
* Relationship among all numerical variables

---

## Hypothesis Testing

### Hypothesis 1

Brand vs Final Price

H₀: Brand has no significant effect on recliner price.

H₁: Brand has a significant effect on recliner price.

Test Used: One-Way ANOVA

Result:

Rejected H₀

Conclusion:

Brand significantly affects recliner prices.

---

### Hypothesis 2

Seater vs Final Price

H₀: Seating capacity has no significant effect on recliner price.

H₁: Seating capacity significantly affects recliner price.

Test Used: One-Way ANOVA

Result:

Rejected H₀

Conclusion:

Seating capacity significantly affects recliner prices.

---

### Hypothesis 3

Discount Percentage vs Final Price

H₀: Discount percentage has no significant relationship with final price.

H₁: Discount percentage significantly relates to final price.

Test Used: Pearson Correlation

Result:

Rejected H₀

Conclusion:

Discount percentage significantly relates to recliner prices.

---

## Key Insights

* Most recliner products belong to the Budget and Mid-Range categories.
* Brown, Beige, and Grey are the most common recliner colors.
* Casacraft from Pepperfry offers the highest number of recliner models.
* Premium brands such as LA-Z-BOY and Durian offer more luxury recliners.
* EMI values increase proportionally with product prices.
* Brand significantly influences recliner pricing.
* Seating capacity significantly affects recliner prices.
* Discounts play an important role in final pricing.

---

## Business Recommendations

* Customers should compare recliners based on price, warranty, and seating capacity rather than relying only on discounts.
* Budget and Mid-Range segments offer the widest variety of recliners.
* Premium brands target customers looking for luxury and high-end products.
* Businesses can optimize pricing strategies by analyzing competitor pricing and discount trends.
* EMI options can be leveraged to improve affordability for higher-priced recliners.

---

## Conclusion

This project demonstrates a complete end-to-end Data Analytics workflow, starting from Web Scraping and Data Collection to Data Preprocessing, Feature Engineering, Exploratory Data Analysis, Hypothesis Testing, and Business Insight Generation.

The analysis identified key factors influencing recliner prices and provided meaningful insights into market trends, customer preferences, and pricing strategies. These findings can support both customers and businesses in making informed decisions within the online furniture market.
