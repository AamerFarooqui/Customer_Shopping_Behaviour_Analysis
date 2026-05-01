# 🛍️ Customer Shopping Behavior Analysis

## 📌 Project Summary
This project analyzes **customer shopping behavior** using transactional data (3,900 records) to uncover insights that help businesses improve **revenue, customer retention, and marketing strategies**.

The project combines **Python, SQL, and Power BI** to transform raw data into actionable business insights.

---

## 🎯 Business Problem
Businesses often struggle to:
- Understand customer purchasing patterns
- Identify high-value customer segments
- Optimize discounts and subscription strategies

👉 This project solves these problems using data-driven insights.

---

## ⚙️ Tech Stack
- **Python** (Pandas, NumPy, Matplotlib, Seaborn)
- **SQL (MySQL)**
- **Power BI**
- Data Cleaning & Feature Engineering
- Exploratory Data Analysis (EDA)

---

## 📊 Dataset Overview
- **Rows:** 3,900  
- **Columns:** 18  
- **Missing Values:** 37 (Review Rating)

### Key Features:
- Customer Demographics (Age, Gender, Location)
- Purchase Details (Item, Category, Amount)
- Behavior Data (Discount, Frequency, Rating, Shipping)

---
## 📁Project Structure

```
customer-shopping-behaviour-analysis/
 
├── dataset/
|   └──customer_shopping_behaviour.csv
|
├── notebook/
│   └── customer_shopping_behaviour.ipynb
│
├── sql/
│   └── customer_behaviour.sql
│
├── dashboard/
|   └──customer_sbehaviour_dashboard.pbix
|
├── report/
│   └── customer shopping behaviour analysis report.pdf
│
└── README.md
```

---
## 🧹 Data Cleaning & Preparation
- Handled missing values using **median imputation (category-wise)**
- Standardized column names (snake_case)
- Removed redundant column (`promo_code_used`)
- Created new features:
  - `age_group`
  - `purchase_frequency_days`

---

## 🔍 Analysis Performed

### 📌 Python (EDA)
- Data distribution analysis
- Feature relationships
- Customer segmentation

### 📌 SQL (Business Queries)
- Revenue by gender
- High-spending discount users
- Top-rated products
- Subscription vs non-subscription analysis
- Shipping impact on purchase value
- Customer segmentation (Loyal, Returning, New)

### 📌 Power BI Dashboard
Built an interactive dashboard showing:
- Revenue trends
- Customer segmentation
- Sales by category
- Age group insights

---

## 📈 Key Insights

### 💰 Revenue Distribution
- Male customers contribute **68% of total revenue**
- Female customers contribute **32%**

### ⭐ Top Rated Products
- Gloves (3.86)
- Sandals (3.84)
- Boots (3.82)

### 🚚 Shipping Insight
- Express shipping users spend more than standard users

### 👥 Customer Segmentation
- Loyal: 79%
- Returning: 18%
- New: 2%

### 🎯 Age Group Revenue
- Young Adults generate highest revenue (~27%)

---

## 📊 Dashboard Preview
<img width="1203" height="675" alt="Dashbord 3" src="https://github.com/user-attachments/assets/100449da-8cb8-4bbb-be05-bddaf150346d" />


---

## 💡 Business Recommendations
- Increase subscription adoption with incentives
- Introduce loyalty programs
- Optimize discount strategies
- Focus marketing on high-value age groups
- Promote top-performing products

---

## 🚀 What I Learned
- End-to-end data analysis workflow
- Writing business-focused SQL queries
- Building interactive dashboards
- Translating data into business insights

---

## 🤝 Contributing

Contributions are welcome! Feel free to fork this repository and submit a pull request.

---

## 📜 License

This project is open-source and available under the MIT License.

---

## 👨‍💻 Author

**Aamer Farooqui**

* GitHub: https://github.com/AamerFarooqui
* LinkedIn: https://www.linkedin.com/in/aamer-farooqui-34b1402ba
---
