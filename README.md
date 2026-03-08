# Customer Shopping Behavior Analysis

## Project Overview

This project analyzes **customer shopping behavior** to uncover insights that can guide strategic business decisions.
The analysis is based on **3,900 purchase records** and focuses on understanding customer demographics, purchasing patterns, revenue distribution, and customer segments.

The goal of this project is to transform raw transactional data into actionable insights that support better business strategies.

---

# Dataset Summary

The dataset used in this project contains:

* **3,900 rows**
* **18 columns**

The dataset includes the following types of information:

### Customer Demographics

* Age
* Gender
* Location
* Subscription Status

### Purchase Details

* Item Purchased
* Category
* Purchase Amount
* Season
* Size
* Color

### Shopping Behavior

* Discount Applied
* Promo Code Used
* Previous Purchases
* Frequency of Purchases
* Review Rating
* Shipping Type

There were **37 missing values in the Review Rating column**.

---

# Data Preparation and Cleaning

## Data Loading

The dataset was imported using **pandas** for further analysis.

## Initial Data Exploration

Initial exploration was performed using:

* `df.info()` to inspect the dataset structure
* `df.describe()` to understand summary statistics

## Missing Data Handling

The **missing values in the Review Rating column** were handled by imputing the **median rating based on product category**.

## Column Standardization

Column names were standardized by converting them into **snake_case format** to improve readability and maintain consistency.

## Feature Engineering

Two additional features were created:

* **age_group** → Created by binning customer ages into groups
* **purchase_frequency_days** → Derived from purchase data

## Data Consistency Check

The variables **discount_applied** and **promo_code_used** were checked for redundancy.
Since they provided overlapping information, **promo_code_used was removed**.

## Database Integration

The cleaned dataset was loaded into **PostgreSQL** by connecting the Python script to the database, allowing SQL-based analysis.

---

# Key Analysis & Insights

## Revenue by Gender

Revenue distribution based on customer gender:

* **Male Customers**

  * Revenue: **$157,890**
  * Contribution: **68% of total revenue**

* **Female Customers**

  * Revenue: **$75,191**
  * Contribution: **32% of total revenue**

---

# Top Products by Rating

The highest-rated products based on average customer ratings are:

1. **Gloves** — Average Rating: 3.86
2. **Sandals** — Average Rating: 3.84
3. **Boots** — Average Rating: 3.82
4. **Hat** — Average Rating: 3.80
5. **Handbag** — Average Rating: 3.78

---

# Shipping and Subscription Insights

## Shipping Type Comparison

Average purchase value based on shipping type:

* **Express Shipping**: $60.48 average purchase
* **Standard Shipping**: $58.46 average purchase

## Subscription Status

**Subscribed Customers**

* Customers: 1,053
* Average Spend: $59.49
* Total Revenue: $62,645

**Non-Subscribed Customers**

* Customers: 2,847
* Average Spend: $59.87
* Total Revenue: $170,436

---

# Discount Dependent Products

Products with the highest percentage of purchases involving discounts:

* **Hat** — 50.00% discounted
* **Sneakers** — 49.66% discounted
* **Coat** — 49.07% discounted
* **Sweater** — 48.17% discounted
* **Pants** — 47.37% discounted

---

# Customer Segmentation

Customers were segmented based on purchasing behavior:

### Loyal Customers

* **79% of customers**
* **3,116 customers**
* Customers with consistent purchase history

### Returning Customers

* **18% of customers**
* **701 customers**
* Customers making occasional purchases

### New Customers

* **2% of customers**
* **83 customers**
* Customers with a single purchase

---

# Revenue by Age Group

Revenue contribution by different age groups:

* **Young Adult** — 27% ($62,143 revenue)
* **Middle-aged** — 25% ($59,197 revenue)
* **Adult** — 24% ($55,978 revenue)
* **Senior** — 24% ($55,763 revenue)

---

# Business Recommendations

## Boost Subscriptions

Promote exclusive benefits and incentives to encourage more customers to subscribe.

## Customer Loyalty Programs

Introduce rewards and loyalty programs to convert returning customers into loyal customers.

## Review Discount Policy

Ensure that discount strategies increase sales while maintaining profit margins.

## Product Positioning

Promote top-rated and best-performing products in marketing campaigns.

## Targeted Marketing

Focus marketing efforts on high-revenue age groups and customers using express shipping.

---
