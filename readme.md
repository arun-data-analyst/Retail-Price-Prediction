# 🛒 Retail Price Prediction Using Machine Learning

Predicting Canadian retail product prices (2017–2025) using:
- 📈 Linear Regression and 🌲 Random Forest Regression
- 🔍 Features: Year, Province, Product Category, Tax Rate

---

## ✅ Key Accomplishments

| Metric     | Linear Regression | Random Forest |
|------------|-------------------|----------------|
| RMSE       | 1.24              | 1.36           |
| R² Score   | 0.94              | 0.93           |

---

## 🔍 Project Overview

This project analyzes historical retail pricing data in Canada (2017–2025) and builds predictive models to estimate **pre-tax product prices**. Exploratory analysis and feature engineering reveal the pricing impact of geography, time, tax structure, and product type.

---

## 📊 EDA Highlights

- **Top 10 Expensive Items**: Infant formula ($32), salmon, and beef rib/striploin cuts.
- **Tax Variation**: Provinces 2–6 showed the highest average tax rates (~15%), while Province 10 had the lowest (~5%).
- **Price Trend**: Average price increased steadily from $4.72 (2017) to $6.44 (2025).
- **Category Spread**: High outliers in 'Meat & Poultry' and 'Infant & Baby Products'.

📁 All visualizations are in the `plots/` folder.

---

## 💡 ML Workflow

- **Target**: `VALUE` (pre-tax retail price)
- **Features**: Year, Month, GEO, Product Category, Products, Taxable, Essential, Total tax rate
- **Preprocessing**: One-hot encoding
- **Modeling**: Linear Regression and Random Forest Regressor
- **Evaluation**: RMSE and R² Score

📌 Predictions visualized in `plots/PredictedVSActual.png`

---

## 📁 Project Structure

```
retail-price-prediction/
│
├── Retail_Project.ipynb               # Main analysis notebook
├── README.md                          # Project summary
├── requirements.txt                   # Required Python packages
├── summary.txt                        # Written insight summary
│
├── data/
│   ├── Retail_Prices_of_Products.csv  # Raw dataset (not uploaded)
│   └── Data_Dictionary.txt            # Column definitions
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

Open `Retail_Project.ipynb` and run all cells in sequence.

---

## 👤 Author

**Arun Acharya**  
Data Analyst in training  
Willis College · Google ML Crash Course Graduate  
📍 Ottawa, Canada

---

## 📌 Tags

`machine-learning` `regression` `retail` `data-analysis` `portfolio-project` `python`
