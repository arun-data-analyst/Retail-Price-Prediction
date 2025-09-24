### 📘 Project Summary: Retail Price Prediction (Canada 2017–2025)
---

#### 🔍 **Objective:**
To build and evaluate machine learning models for estimating the pre-tax retail prices of Canadian products using historical data.

---

#### 📊 **Dataset:**
- **Source:** Kaggle: Product Retail Price Survey (2017–2025)
- **Content:** Prices, taxes, and product details across Canadian provinces.
- **License:** CC0 (Public Domain)

---

#### 📈 **Key Findings from Analysis:**
- **Price Inflation:** Average product prices show a consistent upward trend from 2017 to 2025.
- **High Variability:** 'Infant & Baby Products' and 'Meat & Poultry' have the widest range of prices.
- **Tax Differences:** Provinces 2 through 6 have the highest average tax rates (~15%), while Province 10 has the lowest (~5%).
- **Top-Priced Items:** Premium beef and infant formula are consistently the most expensive products.

---

#### 🤖 **Modeling Results:**
- **Models:** Linear Regression, Random Forest Regression
- **Target Variable:** VALUE (pre-tax price)

- **Linear Regression (Best Performing):**
  - RMSE: 1.24
  - R² Score: 0.94

- **Random Forest Regression:**
  - RMSE: 1.36
  - R² Score: 0.93

---

#### 🧠 **Conclusion:**
Both models performed exceptionally well, but the **Linear Regression** model was slightly more accurate for this dataset. The project successfully demonstrates an end-to-end workflow for solving a real-world pricing estimation problem.