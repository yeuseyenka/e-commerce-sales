# E-commerce Customer Insights | Power BI Dashboard

![Power BI](https://img.shields.io/badge/Power%20BI-Professional-blue?style=flat-square&logo=powerbi)
![DAX](https://img.shields.io/badge/DAX-Advanced-orange?style=flat-square)
![Status](https://img.shields.io/badge/Status-Active-green?style=flat-square)

## 📊 Project Overview

Interactive Power BI dashboard for analyzing customer behavior and lifetime value in e-commerce. The report identifies key demographic segments, evaluates customer satisfaction, and helps determine target groups for retention and upsell actions.

**Data Period:** Jan 2023 – Dec 2025  
**Number of Customers:** 331  
**Total Revenue 2025:** $703,841  

---

## 🎯 Key KPIs 2025

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


## 🔧 Slicers (Filters)

The dashboard includes the following interactive filters:

| Filter | Options |
|--------|---------|
| **Year** | 2025 / 2024 |
| **Category & Product** | All / Specific categories & products |
| **Payment Method** | All / Bank Transfer / Cash on Delivery / Credit Card |
| **City** | All / Specific cities |
| **Age Bin** | All / 18-24, 25-34, 35-44, 45-54, 55-64, 65-74 |
| **Gender** | All / Female / Male / Not disclosed |

Use these slicers to drill down into specific customer segments and analyze their behavior patterns.

---

## 📋 Business Insights

### ✅ Strengths

1. **Youth (18-24) — Most valuable customers:**
   - 47% of total revenue ($331K)
   - High AOV ($769)
   - Good satisfaction score (3.92/5)

2. **High satisfaction** in key categories:
   - Sports & Outdoors: 79% positive ratings
   - Home & Living: 74% positive ratings

3. **Stable customer portfolio:** 331 customers with regular purchase patterns

### ⚠️ Problem Areas

1. **Electronics & Fashion — High negative feedback:**
   - **Electronics:** 13% negative reviews (quality or shipping issues?)
   - **Fashion:** 25% negative reviews (sizing, material, or description mismatches?)

2. **Declining purchase frequency:**
   - **Orders per Customer:** -6.5% over period (2.81 → 2.61)
   - **Action needed:** Implement loyalty program to re-engage customers

3. **Underutilized age groups:**
   - **65-74 age group:** Only 3% of revenue despite 13 customers
   - **Opportunity:** Target with tailored marketing and adapted UX

### 🎯 Strategic Recommendations

| Challenge | Action | Expected Impact |
|-----------|--------|-----------------|
| **Electronics/Fashion quality** | Conduct quality audit, improve descriptions, update product photos | Reduce negative reviews by 30-40% |
| **Youth retention** | Launch referral bonus program (already loyal) | Increase repeat purchases |
| **Older customers** | Create landing page with large fonts, free shipping, special offers | Increase 65-74 segment revenue by 50% |
| **Declining order frequency** | Email campaigns promoting repeat purchases | Reverse -6.5% trend |

---

## 🚀 How to Use

### To View the Report

1. **Download** the `E-commerce Sales.pbix` file from this repository
2. **Open** it in Power BI Desktop (free download at [powerbi.microsoft.com](https://powerbi.microsoft.com))
3. **Explore** using the interactive slicers on the left panel:
   - Filter by age groups, categories, cities, and gender
   - Hover over charts for tooltips
   - Click to cross-filter between visuals

---

## 📞 Contact & License

**Author:** [Eugene Yeuseyenka](https://github.com/yeuseyenka)  
**Email:** [eyeuseyenka@gmail.com](mailto:eyeuseyenka@gmail.com)  
**LinkedIn:** [Eugene Yeuseyenka](https://www.linkedin.com/in/eugene-yeuseyenka/)

**License:** MIT License — free to use for education, portfolio, and commercial purposes.

---

## 🔗 Helpful Resources

- [Power BI Official Documentation](https://docs.microsoft.com/en-us/power-bi/)
- [DAX Function Reference](https://dax.guide/)
- [Power Query M Language Guide](https://docs.microsoft.com/en-us/powerquery-m/)
- [McKinsey on Customer Experience](https://www.mckinsey.com/business-functions/marketing-and-sales/our-insights)

---

## 📊 Changelog

| Version | Date | Updates |
|---------|------|---------|
| 1.0 | 29 Dec 2025 | Initial dashboard release |
| — | — | Not planned |

---

**Last Updated:** 29 Dec 2025  
**Status:** ✅ Active and Maintained  
**Next Update:** Not planned
