# E-commerce Customer Insights | Power BI Dashboard

![Power BI](https://img.shields.io/badge/Power%20BI-Professional-blue?style=flat-square&logo=powerbi)
![DAX](https://img.shields.io/badge/DAX-Advanced-orange?style=flat-square)
![Status](https://img.shields.io/badge/Status-Active-green?style=flat-square)

## 📊 Project Overview

Interactive Power BI dashboard for analyzing customer behavior and lifetime value in e-commerce. The report identifies key demographic segments, evaluates customer satisfaction, and helps determine target groups for retention and upsell actions.

**Data Period:** Jan 2025 – Dec 2025  
**Number of Customers:** 331  
**Total Revenue:** $703,841  

---

## 🎯 Key KPIs

| Metric | Value | Trend |
|--------|-------|-------|
| **Customers** | 331 | ↑ +1.5% (+5) |
| **Average Review Score** | 3.9 | ↓ -2.5% (-0.1) |
| **Sales per Customer** | $2,126 | ↑ +0.3% (+$7) |
| **Orders per Customer** | 2.81 | ↓ -6.5% (-0.20) |

---

## 📈 Main Visuals

### 1. **Sales Summary by Age Bin**
Detailed table broken down by age groups:
- Total Sales, Sales per Customer, Orders per Customer
- Average Order Value (AOV), Average Review Score
- Identifies age cohorts with highest revenue (18-24: $331.5K)

### 2. **Customer Value Segmentation** (Scatter Plot)
- **X-axis:** Average Order Value (AOV)  
- **Y-axis:** Orders per Customer  
- **Size/Color:** Total Sales per customer  
- **Clusters:**
  - 🔵 **High-Value Loyal:** 18-24 (young buyers with frequent purchases)
  - 🟠 **One-Time Big Spenders:** 45-54, 35-44 (infrequent but large orders)
  - 🟡 **Low-Value:** 65-74 (few purchases and small order value)

### 3. **Customer Review Scoring** (Diverging Stacked Bar)
Distribution of ratings (1-5 stars) by category:
- 🔴 **Negative (1-2)** | ⚫ **Neutral (3)** | 🟢 **Positive (4-5)**
- **Problem Categories:** Electronics (13% negative), Fashion (25% negative)
- **Strengths:** Sports & Outdoors (79% positive), Home & Living (74%)

### 4. **Sales by Age & Gender** (Clustered Column)
Comparison of sales by age groups and gender:
- **Legend:** Female (F), Male (M), Not disclosed
- **Insight:** Youth (18-24) leads in revenue; older age groups are underutilized

---

## 💾 Technical Details

### Tools & Technologies
- **BI Platform:** Power BI Desktop / Service  
- **Language:** DAX (Data Analysis Expressions)  
- **Data Preparation:** Power Query (M language)  
- **Database:** Excel / CSV  
- **Version Control:** Git / GitHub  

### DAX Measures Used

```dax
Total Orders := COUNTROWS('Online Retail')

Distinct Customers := DISTINCTCOUNT('Online Retail'[customer_id])

Orders per Customer := DIVIDE([Total Orders], [Distinct Customers])

Average Order Value per Customer := DIVIDE([Total Revenue], [Distinct Customers])

Negative % := DIVIDE(
    CALCULATE(COUNTROWS('Online Retail'), 'Online Retail'[review_score] IN {1, 2}),
    CALCULATE(COUNTROWS('Online Retail'), NOT ISBLANK('Online Retail'[review_score]))
) * 100
Slicers (Filters)
Year: 2025

Category & Product: All / Specific

Payment Method: All / Card / Cash

City: All / Specific cities

Age Bin: All / 18-24, 25-34, 35-44, 45-54, 55-64, 65-74

Gender: All / Female / Male / Not disclosed

📋 Business Insights
✅ Strengths
Youth (18-24) — Most valuable customers:

47% of total revenue ($331K)

High AOV ($769)

Good satisfaction score (3.92/5)

High satisfaction in Sports & Outdoors and Home & Living categories (79% and 74% positive ratings)

Stable portfolio: 331 customers with regular purchases

⚠️ Problem Areas
Electronics & Fashion — High share of negative reviews:

Electronics: 13% negative (quality? shipping issues?)

Fashion: 25% negative (size, material?)

Declining Orders per Customer: -6.5% over period

Customers ordering less frequently (2.81 → 2.61)

Loyalty program implementation needed

Underutilized age groups:

65-74: only 3% of revenue with 13 customers

Opportunity: targeted campaigns, adapted UX

🎯 Recommendations
For Electronics/Fashion: conduct quality audit, improve product descriptions, update photos

For youth (18-24): implement referral bonus program (they're already loyal)

For older customers: create landing page with large fonts, free shipping, special offers

General: launch email campaign promoting repeat purchases (combat -6.5% decline in Orders per Customer)

📂 File Structure
text
📁 ecommerce-powerbi-insights/
├── 📄 README.md (this file)
├── 📊 E-commerce-Customer-Insights.pbix (Power BI file)
├── 📸 screenshots/
│   ├── dashboard-overview.png
│   ├── customer-segmentation.png
│   └── review-scoring.png
└── 📝 notes.md (additional notes, DAX formulas)
🚀 How to Use
To View the Report
Download the E-commerce-Customer-Insights.pbix file

Open in Power BI Desktop (free download at powerbi.microsoft.com)

Refresh the data source if needed (if connected to a database or Excel)

Use the slicers on the left to filter by categories, age groups, cities

To Edit/Adapt
Edit DAX measures in Home → Manage Metrics

Change the data source (Home → Transform data)

Add new visuals, slicers, or measures as needed

Publish to Power BI Service for online access (File → Publish)

📞 Contact & License
Author: Eugene Yeuseyenka
Email: your.email@example.com
LinkedIn: Link to your profile

License: MIT License — free to use for education and portfolio purposes.

🔗 Relevant Links
Power BI Documentation

DAX Function Reference

Power Query M Reference

Last Updated: 29 Dec 2025 | Status: ✅ Active and Maintained
