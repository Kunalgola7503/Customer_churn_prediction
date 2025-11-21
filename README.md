📊 Customer Churn Prediction (Telecom Dataset)
👤 Author: Kunal Gola
🏢 Organization: Codec Technologies (Internship Project)
📁 Project Type: End-to-End Machine Learning + EDA + ML Modeling + Power BI Dashboard
⭐ Project Overview

Customer churn refers to customers stopping the use of a company’s service.
Telecom companies face major losses due to churn, so predicting which customers are likely to leave helps improve retention and revenue.

This project builds a machine learning model that predicts whether a customer will Churn (Yes/No) and also includes a Power BI dashboard to visualize churn patterns and business insights.

🎯 Key Objectives

✔ Perform detailed Exploratory Data Analysis (EDA)
✔ Clean and preprocess telecom churn dataset
✔ Encode categorical features
✔ Train multiple ML models
✔ Select the best model (Gradient Boosting)
✔ Save final model as .pkl
✔ Build a Power BI dashboard using churn data
✔ Prepare a complete project for GitHub & Internship submission

📂 Project Structure
customer-churn-prediction/
│── data/
│    ├── customer_churn_telecom_services.xlsx
│    ├── cleaned_churn.csv
│
│── notebooks/
│    ├── 01_Churn_EDA.ipynb
│    ├── 02_Churn_Modeling.ipynb
│
│── models/
│    ├── churn_model.pkl
│
│── powerbi_dashboard/
│    ├── churn_dashboard.pbix (Power BI file)
│
│── README.md

🧠 Dataset Information

Dataset includes:

Demographics (gender, partner, dependents)

Services (internet, device protection, phone, etc.)

Contract info (month-to-month, one year, two year)

Payment method

Monthly & total charges

Churn flag (Yes/No)

🧹 Data Cleaning & Preprocessing

✔ Converted TotalCharges to numeric
✔ Filled missing values
✔ Removed unnecessary columns (customerID)
✔ Encoded categorical variables using LabelEncoder
✔ Standardized numeric columns
✔ Split into train/test datasets

📊 Exploratory Data Analysis (EDA)

EDA included:

Churn distribution

Tenure distribution

Monthly charges distribution

Churn by gender

Churn by contract type

Churn by payment method

Correlation heatmap

Internet service vs churn

🤖 Machine Learning Models

Models trained:

Logistic Regression

Random Forest

Gradient Boosting (Final Best Model)

Gradient Boosting performed the best in:

Accuracy

Precision

Recall

ROC-AUC

📦 Saving the Model
joblib.dump(gb, "churn_model.pkl")


Load the model:

model = joblib.load("churn_model.pkl")

📈 Model Evaluation

Evaluation metrics:

Accuracy

Precision

Recall

F1-score

ROC-AUC

Confusion Matrix

Feature Importance

Top Predictors of Churn:

Contract Type

Tenure

Monthly Charges

Internet Service

Payment Method

📊 Power BI Dashboard (Key Component)

A Power BI dashboard is created using cleaned_churn.csv to give business-level insights.

Dashboard Includes:

✔ Overall Churn Rate
✔ Churn by Gender
✔ Churn by Contract Type
✔ Churn by Payment Method
✔ Churn vs Tenure Analysis
✔ Monthly Charges: High vs Low churners
✔ Service adoption impact (internet, device protection, tech support)
✔ Slicers for Contract, Gender, Payment Method

Dashboard Purpose:

Understand churn drivers visually

Help business teams identify high-risk customer groups

Provide actionable insights for customer retention strategies

The final dashboard file will be added as:

powerbi_dashboard/churn_dashboard.pbix

🚀 How to Run the Project
Install dependencies:
pip install pandas numpy scikit-learn seaborn matplotlib joblib

Run Notebooks:

01_Churn_EDA.ipynb

02_Churn_Modeling.ipynb

For Power BI:

Open Power BI Desktop

Load cleaned_churn.csv

Build dashboard with charts mentioned above

Save as churn_dashboard.pbix
