# Czech Newspaper Retail Market – Strategic Case Study

This project is based on a second-round interview case study. It analyzes the strategic and operational challenges faced by a fictional newspaper retail company operating in the Czech Republic.

## 📊 Objective

The analysis aims to answer four key business questions:

1. **Estimate the potential of each store**  
   Identify which store-level factors most influence profitability, and suggest additional metrics the company could track.

2. **Decide on underperforming stores**  
   Based on data, determine if there are stores that should be closed or show significant room for improvement.

3. **Cross-selling potential**  
   Analyze how key product categories interact and identify where cross-selling opportunities exist.

4. **Profit mass growth strategies**  
   Suggest actions that could increase overall profit, based on sales, GM (gross margin), and product-level trends.

---

## 🧠 Approach

- Cleaned and validated three data tables:
  - `Forgalom` (Sales & GM by category and time)
  - `Bolttörzs` (Store-level attributes)
  - `Költségek` (Store-level cost data)

- Aggregated data at store-year level and store average level

- Built correlation matrices to find key profitability drivers

- Trained multiple linear regression models to estimate **potential profit** for each store

- Labeled stores by **utilization**: actual profit vs. predicted potential

- Explored product category interactions (correlation & visualization)

- Proposed profit growth strategies using:
  - Seasonal trends
  - Product category contributions
  - Cross-selling patterns

---

## 📂 Files

- `Cseh hírlappiac adattábla.xlsx`: Source dataset
- `Stratégiai dilemmák a cseh hírlappiacon.docx`: Business context and case instructions
- `IFUA_elemzes.ipynb`: Jupyter Notebook with full analysis pipeline (data cleaning → modeling → visualization)
- `README.md`: You are here

---

## 📝 Disclaimer

> ⚠️ **Note**: This project is based on a second-round interview task. The data is fictional and used solely for educational and portfolio purposes. If requested, the repository will be removed.

---

## 🛠️ Tech Stack

- Python
  - `pandas`, `numpy`
  - `matplotlib`
  - `scikit-learn`

---

## 💡 Potential Improvements

- Incorporate external data (e.g., foot traffic, weather, holidays)
- Add clustering for store segmentation
- Deploy as a lightweight dashboard using `Streamlit` or `Dash`

---

## 📬 Contact

Feel free to connect or reach out on [LinkedIn](https://www.linkedin.com/in/nagy-boldizsar0518) if you're interested in discussing the case or data-driven retail strategy.
