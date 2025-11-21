# 📊 **Customer Churn Prediction – Telecom Industry**

### 👨‍💻 **Author:** *Kunal Gola*  
### 🏢 **Organization:** *Codec Technologies – Internship Project*  
### 🔥 **Project Type:** *End-to-End Machine Learning + EDA + Power BI Dashboard*

---

# ⭐ **Project Overview**

Customer churn refers to when customers discontinue a service.  
Telecom companies suffer significant revenue loss when customers leave unexpectedly.

This project builds a **machine learning model** that predicts whether a customer will churn (**Yes/No**), supported by a powerful **Power BI dashboard** to help business teams identify churn patterns and take data-driven decisions.

---

# 🎯 **Project Goals**

- ✔ Perform deep **Exploratory Data Analysis (EDA)**  
- ✔ Clean & preprocess telecom churn dataset  
- ✔ Encode categorical variables  
- ✔ Build multiple ML models  
- ✔ Select **Gradient Boosting** as best model  
- ✔ Save model as `.pkl` for deployment  
- ✔ Build an interactive **Power BI dashboard**  
- ✔ Publish project for GitHub + LinkedIn + internship submission  

---

# 📁 **Project Structure**

```
customer-churn-prediction/
│── data/
│   ├── customer_churn_telecom_services.xlsx
│   ├── cleaned_churn.csv
│
│── notebooks/
│   ├── 01_Churn_EDA.ipynb
│   ├── 02_Churn_Modeling.ipynb
│
│── models/
│   ├── churn_model.pkl
│
│── powerbi_dashboard/
│   ├── churn_dashboard.pbix
│
│── README.md
```

---

# 📚 **Dataset Details**

This dataset includes:

- 👥 Customer demographics  
- 📡 Telecom services usage  
- ⏳ Tenure  
- 💳 Billing & payment information  
- 💰 Monthly & total charges  
- ❗ Churn label (Yes/No)

---

# 🧹 **Data Cleaning & Preprocessing**

Performed:

- ➤ Converted `TotalCharges` → numeric  
- ➤ Removed `customerID`  
- ➤ Filled missing values  
- ➤ Encoded categorical columns  
- ➤ Scaled numerical features  
- ➤ Splitted data into train/test  

---

# 📊 **Exploratory Data Analysis (EDA) Highlights**

Some key findings:

- 🔸 Month‑to‑month contract customers churn the most  
- 🔸 Customers using **Electronic Check** churn heavily  
- 🔸 Lower tenure = higher churn  
- 🔸 Fiber optic users churn more  
- 🔸 High monthly charges increase churn likelihood  

Multiple visualizations were created using **Matplotlib + Seaborn**.

---

# 🤖 **Machine Learning Models Used**

| Model | Result |
|-------|--------|
| Logistic Regression | Good baseline |
| Random Forest | High accuracy |
| 🌟 Gradient Boosting | **Best model** |

The final model:

```
GradientBoostingClassifier()
```

Saved using:

```
joblib.dump(gb, "churn_model.pkl")
```

---

# 📈 **Model Evaluation Metrics**

- ✔ Accuracy  
- ✔ Precision  
- ✔ Recall  
- ✔ F1‑Score  
- ✔ ROC‑AUC  
- ✔ Confusion Matrix  
- ✔ Feature Importance  

**Top Features Influencing Churn:**

- Contract Type  
- Tenure  
- Monthly Charges  
- Payment Method  
- Internet Service  

---

# 📊 **Power BI Dashboard**

An interactive **Power BI Dashboard** is built using `cleaned_churn.csv`.

### Dashboard Includes:

- 🔹 Overall Churn Rate  
- 🔹 Churn by Gender  
- 🔹 Churn by Contract Type  
- 🔹 Churn by Payment Method  
- 🔹 Churn vs Tenure  
- 🔹 Monthly Charges Analysis  
- 🔹 Service‑wise Churn Breakdown  
- 🔹 Dynamic filters (gender, contract, internet service, payment method)

### Dashboard Purpose:

- Identify high‑risk customer segments  
- Understand churn causes visually  
- Support data‑driven retention strategies  



<p align="center"><b>🔥 Completed with Machine Learning + Analytics + BI Excellence</b></p>
