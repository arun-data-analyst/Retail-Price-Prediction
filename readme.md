# 🛒 Retail Price Prediction Using Machine Learning

Predicting Canadian retail product prices (2017–2025) using:

- 📈 **Linear Regression** and 🌲 **Random Forest Regression**
- 🔍 Features: Year, Province, Product Category, Tax Rate, and more

---

## ✅ Key Accomplishments

| Metric   | Linear Regression | Random Forest |
|----------|-------------------|----------------|
| RMSE     | 1.24              | 1.36           |
| R² Score | 0.94              | 0.93           |

---

## 🔍 Project Overview

This project analyzes historical Canadian retail pricing data (2017–2025) to estimate **pre-tax product prices**. It applies supervised learning models and exploratory analysis to uncover how pricing varies by product category, location, time, and tax structure. Built to demonstrate end-to-end applied machine learning for real-world decision support.

---

## 📊 EDA Highlights

- 🍼 **Top Expensive Items:** Infant formula ($32), salmon, and beef rib/striploin cuts
- 🧾 **Tax Variation:** Provinces 2–6 showed the highest average tax (~15%), while Province 10 had the lowest (~5%)
- 📈 **Price Trend:** Average price rose steadily from **$4.72 (2017)** to **$6.44 (2025)**
- 📦 **Category Spread:** ‘Meat & Poultry’ and ‘Infant & Baby Products’ had the highest price variability

📁 Visualizations are saved in the [`plots/`](./plots) folder.

---

## 🤖 ML Workflow

- **Target:** `VALUE` (pre-tax retail price)
- **Features Used:** Year, Month, GEO, Product Category, Product Name, Taxable, Essential, Total Tax Rate
- **Preprocessing:** One-hot encoding of categorical features
- **Models Applied:** 
  - `LinearRegression()` from `sklearn`
  - `RandomForestRegressor()` from `sklearn`
- **Evaluation Metrics:** RMSE and R² Score

📌 See visual results in `plots/PredictedVSActual.png`

---

## 🗂️ Project Structure

```
retail-price-prediction/
│
├── Retail_Project.ipynb               # Main Jupyter notebook
├── readme.md                          # Project summary (this file)
├── requirements.txt                   # Python dependencies
├── summary.txt                        # Short findings summary
│
├── data/
│   ├── Retail_Prices_of_Products.csv  # Full dataset (cleaned)
│   └── Data_Dictionary.txt            # Column descriptions
│
├── plots/
│   ├── boxplot_by_category.png
│   ├── tax_by_province.png
│   ├── top10_expensive_products.png
│   ├── yearly_trend.png
│   └── PredictedVSActual.png
```

---

## 🛠️ How to Run

```bash
pip install -r requirements.txt
jupyter notebook
```

Open `Retail_Project.ipynb` and run all cells to reproduce results.

---

## 👤 Author

**Arun Acharya**  
📍 *Ottawa, Canada*  
🎓 *Data Analyst in Training @ Willis College*  
📘 *Google ML Crash Course*

---

## 🔖 Tags

`machine-learning` `regression` `retail` `data-analysis` `portfolio-project` `python`

---

## 📄 License

This project is licensed under the [MIT License](./LICENSE).