# Retail Sentiment & Revenue Optimization Dashboard

### A Strategic Framework for Pricing and Promotional Analytics

![Status](https://img.shields.io/badge/Status-Complete-success) ![Power BI](https://img.shields.io/badge/Platform-Power_BI-yellow) ![Domain](https://img.shields.io/badge/Domain-Retail_Strategy-blue)

---

## 1. Executive Summary

In high-volume e-commerce environments, standard performance metrics (Average Review Score, Gross Sales) often mask critical underlying variances in customer experience. This project introduces an advanced analytics framework designed to **bridge the gap between volume-centric reporting and qualitative sentiment distribution.**

By leveraging **Diverging Stacked Bar** logic and custom DAX measures, this solution allows stakeholders to move beyond simple averages. It identifies polarized product categories—those with high volatility (simultaneous high negative and high positive feedback)—to enable targeted pricing strategies, inventory rationalization, and promotional allocation.

---

## 2. Business Problem & Solution

### The Challenge
Standard reporting aggregates customer ratings into simple averages (e.g., "3.8/5 Stars"). This approach fails to distinguish between:
* **Stable Mediocrity:** A product where all users rate it a "3".
* **High Polarization:** A product where 50% rate "1" and 50% rate "5".

The latter represents a high-risk, high-reward segment that requires a completely different strategic approach than the former.

### The Analytical Solution
This dashboard implements a **Sentiment Polarity Model** that:
1.  **Visualizes Variance:** Replaces standard box plots with **Diverging Stacked Bar Charts** to align customer sentiment around a neutral baseline.
2.  **Segments Categories:** Isolates "Consistent Winners" (High 4s/5s) for price premiums vs. "Polarized Segments" (High 1s/5s) for quality intervention.
3.  **Directs Strategy:** Provides clear signals for which categories warrant marketing spend versus those requiring operational fixes.

---

## 3. Key Insights & Case Study

Based on the `synthetic_online_retail_data.csv` analysis, the dashboard revealed critical insights regarding the **Sports & Outdoors** category:

* **Observation:** While maintaining a competitive average score, this category exhibited the highest **Polarity Index**. It captured the highest percentage of positive sentiment (77.5%) but also the highest negative sentiment (15.5%), with minimal neutral feedback.
* **Strategic Implication:** The category is not "average"; it is "controversial."
* **Recommendation:**
    * **For Positive SKU clusters:** Implement premium pricing strategies.
    * **For Negative SKU clusters:** Initiate root-cause analysis on returns and defects immediately.
    * **Promotion:** High suitability for targeted ad campaigns due to strong brand advocates, provided specific low-quality SKUs are filtered out.

---

## 4. Technical Architecture

### Data Source
* **Dataset:** `synthetic_online_retail_data.csv`
* **Volume:** ~2,700 Transactional records including customer demographics, order details, and discrete review scores (1-5).

### Analytical Stack
* **Visualization:** Power BI Desktop
* **Data Transformation:** Power Query (M).
* **Modeling:** DAX (Data Analysis Expressions)

### Key DAX Methodologies
The core visualization relies on a calculated **Diverging Scale**:
* **Negative Sentiment (Scores 1 & 2):** Converted to negative values to plot left of the Y-axis.
* **Neutral Sentiment (Score 3):** Bisected (50/50 split) across the axis to minimize visual bias.
* **Positive Sentiment (Scores 4 & 5):** plotted positively to visualize net satisfaction breadth.
