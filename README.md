# Warehouse-and-Retail-Sales-Forecasting
This project aimed to develop a robust, accurate, and interpretable pipeline for forecasting monthly warehouse sales, leveraging historical sales data. By following industry best practices in data cleaning, feature engineering, and machine learning, I produced a model that supports improved inventory planning and business strategy.

# Warehouse & Retail Sales Forecasting

Forecast warehouse sales using machine learning to support inventory management, supplier strategy, and operational planning.

## 📈 Project Overview

This repository contains a complete pipeline for predicting monthly warehouse sales using historical sales data. The project demonstrates end-to-end data science best practices, from data cleaning to feature engineering, modeling, evaluation, and deployment.

## 🧐 Business Questions

- Can we accurately forecast monthly warehouse sales for better planning?
- Which factors (supplier, item type, time/seasonality) drive sales volume?
- How can predictive modeling help optimize inventory and supplier relations?

## 🗃️ Dataset

- **Source:** Internal company data (`Warehouse_and_Retail_Sales.csv`)
- **Rows:** 307,645
- **Columns:** YEAR, MONTH, SUPPLIER, ITEM CODE, ITEM DESCRIPTION, ITEM TYPE, RETAIL SALES, RETAIL TRANSFERS, WAREHOUSE SALES
- **Ethical Considerations:** No customer/PII data. Follow internal and external data privacy policies. Mask/anonymize supplier/product names if needed for public sharing.

## 🛠️ Methodology & Tools

- **EDA:** Exploratory data analysis, outlier and missing value checks, visualizations
- **Data Cleaning:** Drop missing values, remove negative outlier sales
- **Feature Engineering:** Aggregation and one-hot encoding for categorical features (supplier, item type)
- **Modeling:** Linear Regression (baseline), Random Forest Regression (primary), hyperparameter tuning with GridSearchCV
- **Evaluation:** RMSE, MAE, R², actual vs predicted plots, residuals analysis, overfitting checks
- **Prediction & Deployment:** Predict new sales and save best model for future use

**Tools:**  
Python, pandas, numpy, matplotlib, seaborn, scikit-learn, joblib, Jupyter Notebook

## 🗓️ Project Timeline

| Week | Milestone                                  |
|------|--------------------------------------------|
| 1    | Project kickoff and EDA                    |
| 2    | Data cleaning & feature engineering        |
| 3    | Model development & baseline evaluation    |
| 4    | Model tuning, validation, interpretation   |
| 5    | Final reporting & demo delivery            |

See `/Warehouse_and_Retail_Sales_Project_Timeline.png` for Gantt chart.

## 🚀 Results

- **Best Model:** Tuned Random Forest Regressor
    - **Test R²:** 0.98
    - **Test RMSE:** 809
    - **No significant overfitting detected**
- **Key Drivers:** Supplier, item type, and seasonality (month/year) are most influential for warehouse sales.

## 📂 Files

- `Warehouse_and_Retail_Sales_Cleaned_Modeling.ipynb` – Complete, reproducible analysis and modeling notebook
- `Warehouse_and_Retail_Sales_Project_Plan.docx` – Project plan (Word document)
- `Warehouse_and_Retail_Sales_Project_Timeline.png` – Gantt chart
- `Warehouse_and_Retail_Sales.csv` – Input data (not included in public repo; add your own)
- `tuned_random_forest_model.joblib` – Saved model (generated after running notebook)

## 📝 Recommendations

- Retrain model regularly with new data
- Monitor data quality and retrain as needed
- Consider adding features (promotions, holidays, external factors) for even better accuracy
- Expand to other sales channels as business needs evolve

## 👨‍💻 Getting Started

1. Clone the repository
2. Add your own `Warehouse_and_Retail_Sales.csv` file to the root folder
3. Open and run `Warehouse_and_Retail_Sales_Cleaned_Modeling.ipynb` in Jupyter Notebook
4. Follow notebook instructions to reproduce results and make new predictions

## 📢 License & Contact

- Stephen Nnamani
- For inquiries, reach out via GitHub issues

---

*This project is for demonstration/educational purposes and does not contain proprietary or confidential customer data.*
