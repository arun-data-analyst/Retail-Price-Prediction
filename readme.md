# 🛒 Retail Price Prediction Using Machine Learning

[cite_start]This project analyzes historical Canadian retail pricing data (2017–2025) to build and evaluate supervised learning models for estimating pre-tax product prices[cite: 1, 9].

---

## 🎯 Project Goal

[cite_start]The primary objective is to predict the `VALUE` (pre-tax price) of retail goods based on features like the date, province, product category, and tax structure[cite: 1]. [cite_start]This project showcases an end-to-end data analysis workflow, from cleaning and visualization to predictive modeling, making it a strong portfolio piece for data analytics roles[cite: 9].

---

## 🏆 Modeling & Results

Two regression models were trained to predict prices. [cite_start]While both were highly accurate, **Linear Regression** performed slightly better on this dataset[cite: 6].

| Metric | ✅ Linear Regression (Best) | 🌲 Random Forest |
| :--- | :--- | :--- |
| **RMSE** | 1.24 | 1.36 |
| **R² Score** | 0.94 | 0.93 |

- **RMSE (Root Mean Squared Error):** Represents the average prediction error. A lower value is better.
- **R² Score:** Indicates the percentage of price variation the model can explain. A higher value (closer to 1.0) is better.

![Predicted vs Actual Prices Plot](plots/PredictedVSActual_Improved.png)

---

## 🔍 Key Findings & Visualizations

- [cite_start]**Price Inflation Trend:** Average prices rose steadily from **$4.72 in 2017 to $6.44 in 2025**, indicating a clear inflationary trend[cite: 4].
- [cite_start]**Tax Rate Variation:** Provinces 2–6 had the highest average tax rates (~15%), while Province 10 had the lowest (~5%)[cite: 3].
- [cite_start]**Most Expensive Items:** Premium beef cuts and infant formula consistently topped the list of most expensive products on average[cite: 5].
- [cite_start]**Category Price Spread:** ‘Meat & Poultry’ and ‘Infant & Baby Products’ categories showed the greatest price variability and the most outliers[cite: 1].

[cite_start]All visualizations are saved in the [`plots/`](./plots) folder[cite: 8].

---

## 🤖 Machine Learning Workflow

1.  **Preprocessing:** Categorical features (e.g., `GEO`, `Products`) were converted into a numerical format using one-hot encoding.
2.  [cite_start]**Feature Selection:** The following features were used for prediction: `Year`, `Month`, `GEO`, `Product Category`, `Products`, `Taxable`, `Essential`, and `Total tax rate`[cite: 6].
3.  [cite_start]**Model Training:** The data was split (80% train, 20% test) and used to train two models from the `sklearn` library: `LinearRegression()` and `RandomForestRegressor()`[cite: 6].
4.  **Evaluation:** Models were assessed based on their RMSE and R² scores on the unseen test data.

---

## 💡 Conclusion & Next Steps

Both models demonstrated strong predictive power, with the Linear Regression model showing a slight edge in performance. This suggests that the relationships in the data are largely linear and well-captured by this model. [cite_start]Random Forest still offers benefits like resilience to outliers[cite: 7].

**Possible Next Steps:**
- **Hyperparameter Tuning:** Fine-tune the Random Forest model to potentially improve its accuracy.
- **Feature Engineering:** Create new features (e.g., seasonal indicators) to see if model performance can be enhanced.
- **Deployment:** Package the best-performing model into a simple web application or API for real-time price estimations.

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
│   ├── PriceDistributionByCategory.png
│   ├── TaxRateByProvince.png
│   ├── TopMostExpensiveItems.png
│   ├── AveragePriceOverTime.png
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
🎓 *Data Analyst*  

---

## 🔖 Tags

`machine-learning` `regression` `retail` `data-analysis` `portfolio-project` `python`

---

## 📄 License

This project is licensed under the [MIT License](./LICENSE).