# Pakistan E-Commerce Sales Performance & Customer Insights Dashboard

![Dashboard Banner](Images/Business_Performance_Overview.png)

## Project Overview
This project analyzes Pakistan’s largest e-commerce dataset to uncover key trends in **sales performance**, **customer behavior**, and **operational efficiency**.  
The analysis was performed in **Power BI**, leveraging data modeling (Star Schema), DAX measures, and interactive visualizations to drive **actionable business insights** for marketing, pricing, and inventory optimization.

---
![Customer Behavior](Images/Customer_Behavior.png)
## Objectives
1. Identify overall **sales trends and revenue performance** across months and years.  
2. Discover **top-selling product categories** and least-performing items.  
3. Understand **customer acquisition vs. retention** patterns.  
4. Evaluate **payment-method reliability**, cancellations, and return behavior.  
5. Provide **strategic recommendations** for marketing, pricing, and inventory control.

---

## Dataset Description
- **Dataset Source:** *Pakistan E-Commerce Dataset (Kaggle)*  
- **Rows:** ≈ 234,000 transactions  
- **Columns:** 20+ attributes including `item_id`, `customer_id`, `order_status`, `unit_price`, `quantity_ordered`, `payment_method`, `created_at`, etc.  
- **Time Frame:** 2016 – 2018  
- **Currency:** PKR (Pakistani Rupees)

---

## Data Preparation & Modeling
Performed in **Power Query** within Power BI.

| Step | Description |
|------|-------------|
| **Data Cleaning** | Removed nulls · corrected data types · handled date formats |
| **Feature Engineering** | Added Year, Month, Quarter, Financial Year, DateKey |
| **Normalization** | Built Dim tables: `Dim_Date`, `Dim_Customer`, `Dim_Product`, `Dim_Payment` |
| **Fact Table** | `Fact_Sales` — aggregates orders, revenue, discounts, and quantities |
| **Relationships** | One-to-many joins via surrogate keys (Star Schema) |

> **Schema:** `Fact_Sales` ↔ `Dim_Date`, `Dim_Customer`, `Dim_Product`, `Dim_Payment`

---

## Tools & Technologies
- 🟨 **Power BI Desktop / Service** – Data Modeling & Visualization  
- 🧮 **DAX** – Calculated Measures & KPIs  
- 🧰 **Power Query Editor** – ETL Transformation  
- 🗃️ **Excel / CSV** – Data Source Handling  
- 💻 **GitHub & Markdown** – Portfolio Documentation  

---

## Exploratory Data Analysis (EDA)
![Overview](Images/Overview.png)

### 🔹 Overview KPIs
| Metric | Value (PKR) |
|---------|-------------|
| **Total Revenue** | **2.22 B** |
| **Net Revenue (Excl. Discount)** | **2.08 B** |
| **Total Orders** | **234 K** |
| **Total Quantity Sold** | **334 K** |
| **Average Order Value (AOV)** | **9.5 K** |
| **Total Discount** | **133.3 M** |
| **Revenue Growth (2016–2018)** | **6.54 %** |
| **Average CLV** | **46.2 K** |

---

### 🔹 Time Analysis
- **Peak Months:** **February, March, May** (≈ ₨ 0.4 B each)  
- **Yearly Revenue:** 2016 → ₨ 128.9 M | 2017 → ₨ 388.9 M | 2018 → ₨ 1.70 B  
- **Top Categories:** Mobiles & Tablets · Appliances · Entertainment  

![Monthly Revenue Charts](images/Trend_Analysis.png)

**Interpretation:**  
Revenue peaks align with **Eid & summer shopping seasons** (Q1–Q2).  
2018 contributed > 75 % of total sales — a scaling phase for the platform.

---

### 🔹 Customer Insights
- **Top 20 Customers CLV:** ₨ 5.5 M – ₨ 20 M  
- **New Customers ≫ Returning Customers**, especially in March & May.  
- **Total Customers:** ≈ 48 K  

![Customer Trend](images/Customer_Insights.png)

**Insight:** Acquisition is strong, but **retention and repeat purchases** are weak → need for loyalty programs and personalized marketing.

---

### 🔹 Product & Payment Performance
**Return Rate by Payment Method**
| Method | Return Rate |
|---------|-------------|
| Mcblite | 31 % |
| COD | 20 % |
| CustomerCredit | 17 % |

**Cancellation Rate by Payment Method**
| Method | Rate |
|---------|------|
| MyGateway | 100 % |
| UBL Credit Card | 81 % |
| APG | 78 % |
| Internet Banking | 74 % |
| COD | 7 % |
| CustomerCredit | 0 % |

**Interpretation:**  
- COD dominates sales but creates high return risk.  
- Prepaid methods suffer trust issues → need UI improvements & payment education.  
- Pricing and promotions should differentiate between stable vs. risky methods.

---

### 🔹 Order Status & Fulfillment
| Status | Share % |
|---------|---------|
| **Completed** | 35 % |
| **Canceled** | 34 % |
| **Delivered** | 19 % |
| **Refunded** | 11 % |

**Insight:** ~50 % orders don’t complete → fulfillment and logistics optimization needed.

---

## Key Strategic Insights

### Marketing
- Revenue concentrated in Q1–Q2 → schedule major campaigns in Feb–May.  
- Focus on **retention** via loyalty points, personalized emails, and post-purchase offers.  
- Segment customers by **CLV tiers** for targeted marketing.  

### Pricing
- Apply **dynamic pricing** based on seasonality and payment method risk.  
- Offer **prepaid discounts** to reduce COD dependency.  
- Bundle complementary products to raise AOV without margin loss.  

### Inventory & Fulfillment
- Introduce **predictive stock planning** for Q1–Q2 peaks.  
- Track **courier KPIs** (returns, delivery times).  
- Enhance **reverse logistics** to recycle returns quickly.  

---

## Conclusion
The analysis exposes a high-potential but operationally inefficient market.  
To ensure sustainable growth:
1. **Shift from acquisition to retention focus.**  
2. **Promote digital payments** and trust in prepaid methods.  
3. **Adopt data-driven pricing** to balance volume and profit.  
4. **Optimize inventory logistics** to reduce returns and refund losses.

Together, these strategies can **boost profitability**, **improve customer loyalty**, and **stabilize revenue** in Pakistan’s evolving e-commerce sector.

---

## Dashboard Preview
| Overview | Time Analysis | Customer Insights |
|-----------|---------------|------------------|
| ![Overview](Images/Overview.png) | ![Time Analysis](Images/Trend_Analysis.png) | ![Customer Insights](Images/Customer_Insights.png) |

---

## Live Dashboard
🔗 **[View Interactive Power BI Report Here](https://app.powerbi.com/links/7qDR3DSPpR?ctid=b1dda083-00ad-4557-b34b-d2157536982b&pbi_source=linkShare)**

---

## 💼 Author
**Muhammad Raiq Khalil**  
Data Analyst | Power BI Developer  
📧 raiqkhan520@gmail.com 
🌐 [LinkedIn Profile](https://www.linkedin.com/in/muhammad-raiq-khalil/)  
📂 This repository includes: `.pbix`, `.md`, and dashboard screenshots.

---

## License
This project is for portfolio and educational use. Data sourced from public datasets on Kaggle.

---

If you found this analysis useful, consider starring the repository to support future projects!
