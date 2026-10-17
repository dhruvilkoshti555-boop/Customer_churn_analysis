# 📉 Customer Churn Analysis

## 📌 Overview
This project analyzes a telecom customer dataset to find out **who churns, why, and what the business can do about it**. It combines exploratory analysis with a simple churn prediction model.

## 🧰 Tools Used
- Python
- Pandas
- Matplotlib
- Scikit-learn

## 📂 Dataset
`churn.csv`: 7,043 telecom customers with 21 columns covering demographics, services subscribed, contract, billing and whether the customer churned.

## 🔍 Analysis Performed
- Data cleaning (fixing `TotalCharges`, handling missing values, encoding churn as 0/1)
- Overall churn rate
- Churn by contract type, tenure, internet service, tech support and payment method
- Monthly charges and tenure: churned vs retained customers
- Logistic regression model to predict churn (ROC-AUC ≈ 0.84)

## 📈 Key Insights
- Overall churn rate is about **26.6%**
- **Month-to-month** customers churn at ~43%, vs ~11% (1-year) and ~3% (2-year)
- **New customers** are most at risk: ~48% churn within the first 12 months
- **Fiber optic** customers churn at ~42%, more than double DSL (~19%)
- Customers **without tech support** churn at ~42%, vs ~15% with it
- **Electronic check** payers churn at ~45%, vs ~15-19% for other methods

## 💡 Business Recommendations
- Offer incentives to move customers onto 1- and 2-year contracts
- Strengthen onboarding and support in the first 12 months
- Bundle tech support and online security, especially for fiber customers
- Investigate fiber optic service quality and pricing
- Encourage automatic payment methods
- Use the model to flag high-risk customers for retention offers

## ▶️ How to Run
```bash
pip install pandas matplotlib scikit-learn jupyter
jupyter notebook churn_analysis.ipynb
```
Keep `churn.csv` in the same folder as the notebook.

## 📁 Files
| File | Description |
|------|-------------|
| `churn_analysis.ipynb` | Full analysis notebook |
| `churn.csv` | Dataset |
| `README.md` | Project summary |
