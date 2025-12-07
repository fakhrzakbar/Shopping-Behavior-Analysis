# Shopping-Behavior-Analysis
# 🛍️ Retail Sales & Customer Behavior Analysis | Power BI Dashboard

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Data Analysis](https://img.shields.io/badge/Data_Analysis-blue?style=for-the-badge)

## 📸 Dashboard Screenshots

**Page 1: Executive Summary**
*(High-level KPIs, Demographics, and Geographic Performance)*
![Page 1 Executive Summary](https://github.com/fakhrzakbar/Shopping-Behavior-Analysis/blob/main/Screenshot%20(2362).png)

**Page 2: Customer & Operations**
*(Payment Preferences, Loyalty Analysis, and Shipping Trends)*
![Page 2 Customer Operations](https://github.com/fakhrzakbar/Shopping-Behavior-Analysis/blob/main/Screenshot%20(2363).png)

**Page 3: Product & Inventory Deep Dive**
*(Size Sizing Curves, Seasonal Stability, and Pricing Strategy)*
![Page 3 Product Deep Dive](https://github.com/fakhrzakbar/Shopping-Behavior-Analysis/blob/main/Screenshot%20(2364).png)

---

## 1. 📝 Project Overview

**The Goal:**
To transform raw retail transaction data into a strategic business intelligence tool. This project moves beyond simple reporting to diagnose business health, uncover operational inefficiencies, and provide data-backed recommendations to improve margins and inventory strategy.

**The Focus:**
* **Executive Strategy:** Tracking high-level performance (Revenue, AOV) and demographic profiling.
* **Customer Operations:** Analyzing payment friction, shipping logistics, and loyalty program gaps.
* **Inventory Optimization:** Identifying risk in size curves, seasonal variance, and pricing elasticity.

---

## 2. 🛠️ Tools & Technology

* **Microsoft Power BI Desktop:** Used for data visualization and interactive reporting.
* **Power Query:** Performed data cleaning, profiling, and age-binning transformations.
* **DAX (Data Analysis Expressions):**
    * Created complex measures for `Total Revenue`, `Average Order Value`, and `Transaction Counts`.
    * Used `CALCULATE`, `SWITCH`, and `COUNTROWS` for dynamic segmentation.
    * Implemented `TOPN` logic for "Best Seller" dynamic cards.
* **Data Modeling:** Built a Star Schema (optimized) for performance.

---

## 3. 📂 Data Source

* **Dataset:** `shopping_behavior_updated.csv`
* **Volume:** 3,900 Customer Transactions.
* **Key Attributes:** Customer ID, Age, Gender, Item Purchased, Category, Purchase Amount (USD), Location, Size, Color, Season, Review Rating, Subscription Status, Shipping Type, Discount Applied, Promo Code Used, Payment Method.
* **Data Quality:** Verified 100% completeness (no missing values) via Power Query column profiling.

---

## 4. 🔄 Key Analysis Steps

1.  **Data Profiling & Cleaning:**
    * Checked for null values and data type consistency.
    * Created a "Calculated Column" to group individual ages into demographic bins (e.g., "18-24", "25-34").
2.  **Measure Calculation (DAX):**
    * Developed measures for core KPIs to ensure aggregation accuracy.
    * Created logic for "Star Ratings" (converting numbers to ★ symbols).
3.  **Visual Design & UX:**
    * Designed a custom **Left Sidebar Navigation** for an app-like user experience.
    * Implemented a "Drill-Down" journey: *Executive View* $\rightarrow$ *Operational View* $\rightarrow$ *Product Deep Dive*.
    * Used **Conditional Formatting** on the Seasonal Matrix to create heatmaps for trend spotting.
    * Utilized **Decomposition Trees** for root-cause analysis of revenue drivers.

---

## 5. 💡 Key Insights & Recommendations

### 📊 Strategic Pivot (Demographics)
* **Insight:** The customer base is **68% Male**, contradicting typical "female-first" fashion strategies.
* **Action:** Future marketing campaigns should double down on the male demographic (ages 25-54) rather than using generic targeting.

### 📉 The Discount Trap (Pricing)
* **Insight:** Promotional discounts are **ineffective** at increasing basket size. The Average Order Value (AOV) is flat at ~$60 regardless of whether a discount is applied.
* **Action:** Shift strategy from "Flat Discounts" to "Threshold-Based Offers" (e.g., "Save $10 on orders over $100") to force an increase in AOV.

### 📦 Inventory Optimization (Size Curves)
* **Insight:** There is a critical inventory mismatch. **Size Medium** accounts for **45%** of all sales, creating a high risk of stockouts if standard sizing ratios are used.
* **Action:** Implement a **4:3:2:1 Buying Ratio** (M:L:S:XL) for future factory orders.

### ❄️ "Season-Proof" Supply Chain
* **Insight:** Seasonal categories like "Outerwear" show virtually **zero revenue variance** between Summer and Winter.
* **Action:** Move to a "Continuous Production" model rather than "Seasonal Batching" to lower warehousing costs and smooth cash flow.

---

*Created by [M. Fawwawz Akbar] - [https://www.linkedin.com/in/m-fawwaz-akbar/]*
