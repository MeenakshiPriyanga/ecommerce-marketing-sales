# ecommerce-marketing-sales
E-commerce Marketing and sales Problem statement

# 📊 Customer Acquisition Analysis – E-Commerce Case Study

## 🧩 Business Context

An online retail company wants to analyze its customer acquisition patterns over time to identify seasonal trends, optimize marketing strategies, and ensure consistent growth throughout the year. The business aims to uncover which months perform better in acquiring new customers, what factors influence these trends, and how marketing spend aligns with acquisition outcomes.

This analysis will inform strategic decisions such as when to ramp up campaigns, launch promotions, or optimize customer onboarding efforts.

---

## 📁 Data Overview

### 1. `online_sales_data.csv`
- **Rows**: 52,924 transactions
- **Key Variables**: `CustomerID`, `Transaction_Date`, `Product_Category`, `Quantity`, `Avg_Price`, `Coupon_Status`
- Used to identify the first purchase date (i.e., acquisition) per customer.

### 2. `customers_data.csv`
- **Rows**: 1,468 unique customers
- **Key Variables**: `CustomerID`, `Gender`, `Location`, `Tenure_Months`
- Used to cross-validate acquisition timing and segment users demographically.

### 3. `marketing_spend_data.csv`
- **Rows**: 365 (daily)
- **Key Variables**: `Month`, `Offline_Spend`, `Online_Spend`
- Used to analyze correlation between marketing efforts and new customer acquisitions.

---

## 🔍 Exploratory Data Analysis (EDA) Plan

### Business Questions:
- Which months have the highest and lowest customer acquisition rates?
- Are acquisition trends consistent across years?
- How does marketing spend relate to acquisition volume?
- Which months are most cost-effective in terms of Customer Acquisition Cost (CAC)?

### EDA Steps:
1. Convert `Transaction_Date` to datetime and extract `Acquisition_Month`.
2. Group customers by their first transaction to calculate acquisition trends.
3. Merge with marketing spend data to compare acquisition volume with marketing investment.
4. Compute cost per acquisition (CPA) per month.
5. Visualize trends and extract actionable insights.

---

## 📊 Visual Insights

### 🧩 Monthly Customer Acquisition
![Customer Acquisition Bar Chart](images/customer_acquisition.png)

### 🧩 Acquisition vs Marketing Spend
![Spend vs Acquisition](images/spend_vs_acquisition.png)

### 🧩 Cost Per Acquisition (CPA) Trends
![Cost Per Acquisition](images/cpa_trends.png)

---

## 💡 Key Insights

- 📈 **Peak acquisition months** were identified in March and November, likely aligned with seasonal promotions and marketing pushes.
- 📉 **Lowest acquisition** occurred in July and September, with reduced marketing spend and less promotional activity.
- 💸 **Cost per acquisition (CPA)** was lowest during high-acquisition months, indicating higher marketing efficiency.
- 🎯 A mismatch was observed in some months (e.g., high spend but low acquisition), suggesting the need for campaign optimization.

---

## ✅ Recommendations

1. **Capitalize on High-Performing Months**:
   - Increase marketing budget strategically during peak months.
   - Launch exclusive promotions or new products.

2. **Boost Slow Months**:
   - Run targeted campaigns in July and September (email, retargeting).
   - Offer limited-time discounts or bundled offers.

3. **Optimize Marketing Spend**:
   - Track CPA monthly and set thresholds for campaign ROI.
   - Reallocate budget from ineffective months to those with higher potential.

4. **Segment-Based Marketing**:
   - Use customer demographics (from `customers_data`) to personalize campaigns by gender, region, or tenure.

---

## 🛠️ Future Work

- Integrate website traffic or campaign click-through data to track full customer journey.
- Analyze repeat purchases and customer lifetime value (CLV).
- Explore churn trends using `Tenure_Months` and reactivation strategies.

---

📁 *This analysis empowers data-driven decision-making for scalable and sustainable customer acquisition strategies.*

