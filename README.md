# Czech Retail Data Science Case Study

This project was created as part of a second-round interview task.  
The data used is **not real** and serves **only educational and portfolio purposes**.

---

## 📌 Business Objective

The case focuses on analyzing the potential of different retail stores in the Czech Republic based on their financial and operational performance. It includes estimating profitability, identifying underperforming stores, exploring cross-selling opportunities, and proposing actions to increase profit mass.

---

## 📊 Dataset Overview

The Excel file contains three sheets:
- **Store characteristics** (e.g. size, staff, facilities, demographics)
- **Revenue and GM data**
- **Cost data**

---

## 🧠 Methodology

### 1. Data Cleaning
- Missing numerical values were filled with column means.
- Missing categorical values were filled with `"N/A"`.
- Negative or invalid values in features like area were corrected.
- Duplicated rows were dropped.

### 2. Profit Estimation
- Gross Margin (GM) and Costs were aggregated yearly and per store.
- Profit was calculated as `GM + Costs` (costs are negative in the dataset).
- Stores were categorized into:
  - Top 10 by profit
  - Bottom 10 by profit

### 3. Potential Estimation
- A **linear regression model** was trained to predict theoretical profit based on store attributes.
- Predicted profit vs. actual profit was compared → `Utilization = Actual / Predicted`
- This utilization metric was used to identify:
  - Stores that underperform vs. potential
  - High-potential stores worth investment

### 4. Statistical Analysis
- **Correlation matrix** created for all numeric columns.
- Features with correlation > 0.2 with profit were used in regression modeling.
- For **categorical (non-numeric)** features, **ANOVA tests** were conducted to examine the relationship between each category and profit.

### 5. Cross-Selling Opportunities
- Pivot table of GM by product category and month was created.
- Correlation matrix between product categories helped reveal potential cross-selling synergies.

### 6. Profit-Mass Optimization Ideas
- Price or bundle discounts in high-volume but low-GM categories
- Seasonal campaign suggestions based on GM trends
- Store benchmarking for sharing best practices
- Targeted marketing in low-utilization stores

---

## 📈 Visualizations
The project includes:
- Seasonal GM trends by product category
- Pie charts showing GM contribution per category per year
- Scatterplots and correlation heatmaps for feature selection

---

## 📂 File Structure

```
├── IFUA_elemzes.ipynb       # Jupyter Notebook with full analysis
├── Cseh hírlappiac adattábla.xlsx  # Provided Excel file
├── IFUA_masodik_fordulo.pptx       # Final business presentation
└── README.md                # This file
```

---

## ✅ Key Results

- Clear underperformance identified in ~10% of stores
- Regression R² = ~0.82 using selected store features
- Strong predictors of profit: store size, weekly opening hours, location
- Product categories with cross-selling potential: [example if available]
- Several store-specific and company-wide actions proposed

---

## 🔐 Disclaimer

This repository was created based on a case study given during a job interview.  
**All data is fictitious** and any resemblance to real entities is purely coincidental.

---