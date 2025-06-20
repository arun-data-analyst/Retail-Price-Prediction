# 🛒 Retail Price Prediction Using Machine Learning

This project analyzes historical retail pricing data in Canada (2017–2025) and builds predictive models to estimate product prices based on features like year, province, product category, and tax structure. Using both Linear Regression and Random Forest Regression, it explores pricing trends, tax variations, and the impact of product type on retail value. This project combines practical data analysis and machine learning to support pricing insights, business decisions, and entry-level data analyst portfolio development.

---

## 📁 Dataset

- **Source:** [Kaggle - Product Retail Price Survey (2017–2025)](https://www.kaggle.com/datasets/aradhanahirapara/product-retail-price-survey-2017-2025)
- **Author:** Aradhana Hirapara
- **License:** [CC0: Public Domain](https://creativecommons.org/publicdomain/zero/1.0/)
- **File:** `Retail_Prices_of _Products.csv`

---

## 🎯 Project Goals

- Predict the **pre-tax retail price** of a product using historical data
- Explore relationships between product type, geography, and price
- Demonstrate regression modeling with real-world data

---

## 🔍 Exploratory Data Analysis (EDA)

1. **Boxplot:** Price distribution across product categories\
   → Categories like 'Infant & Baby Products' and 'Meat & Poultry' showed high variability and outliers, while staples like 'Frozen Foods' and 'Canned Goods' had more stable pricing.

2. **Barplot:** Total tax rate by province (GEO)\
   → Provinces 2–6 showed the highest average tax rates (\~15%), while Province 10 had the lowest (\~5%). The remaining provinces fell in the mid-range (11–13%).

3. **Lineplot:** Yearly average price trend (2017–2025)\
   → Indicated a general upward trend in average product prices over time, consistent with inflation.

4. **Barplot:** Top 10 most expensive products (on average)\
   → Infant formula, beef cuts (rib, striploin, sirloin), and salmon were among the highest-priced products. These findings highlight premium categories that influence retail strategy.

Visuals saved in the `plots/` folder.

> **Note:** Some EDA ideas were inspired by public Kaggle notebooks shared under CC licenses. All code and visualizations were recreated and modified independently.

---

## 🧠 Machine Learning

- **Models Used:**
  - Linear Regression (sklearn)
  - Random Forest Regression (sklearn)

Both models were trained and evaluated. Random Forest Regression was added to improve robustness by capturing non-linear relationships in the data.

**Performance Metrics:**

- Linear Regression:

  - RMSE: \~1.24
  - R² Score: \~0.94

- Random Forest Regression:

  - RMSE: \~1.36
  - R² Score: \~0.93

- **Target:** `VALUE` (pre-tax price)

- **Features used:** Year, Month, GEO, Product Category, Products, Taxable, Essential, Total tax rate

- **Data Prep:** One-hot encoding of categorical features

- **Evaluation Metrics:**

  - RMSE: \~1.24
  - R² Score: \~0.94 (excellent fit)

---

## 🚀 Files Included

```
retail-price-prediction/
│
├── Retail_Project.ipynb               # Main Jupyter notebook
├── README.md                          # This file
├── requirements.txt                   # Required Python packages
├── data/
│   └── Retail_Prices_of _Products.csv # Dataset file
├── plots/
│   ├── boxplot_by_category.png
│   ├── tax_by_province.png
│   ├── yearly_trend.png
│   └── top10_expensive_products.png
```

---

## 🛠️ How to Run

```bash
pip install -r requirements.txt
jupyter notebook
```

Open `Retail_Project.ipynb` and run the cells.

---

## 👤 Created by

**Arun Acharya** — Data Analyst in training (Willis College & Google ML Crash Course)

📌 *Portfolio project to showcase applied machine learning in the retail industry.*

