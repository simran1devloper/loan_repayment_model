# 🏦 Loan Repayment Prediction System

## 📌 Project Objective
The goal of this project is to build an AI-driven system that predicts whether a borrower will **repay a loan on time or default**. This helps **banks, financial institutions, and fintech companies** assess borrower risk before approving loans.

---

## 🔹 Dataset: Kaggle Loan Default Prediction Dataset
A commonly used dataset for loan repayment prediction is the **“Home Credit Default Risk”** dataset from Kaggle.

📌 **Dataset URL:** [Kaggle Loan Default Dataset](https://www.kaggle.com/c/home-credit-default-risk)

### 📊 Features in the Dataset:
The dataset contains borrower information, loan details, and past financial behavior.

| Feature Name              | Description |
|---------------------------|------------|
| **TARGET**                | 1 = Loan Default, 0 = Repaid Loan |
| **AMT_CREDIT**            | Loan amount requested |
| **AMT_ANNUITY**           | Annual repayment amount |
| **AMT_INCOME_TOTAL**      | Total annual income of borrower |
| **DAYS_EMPLOYED**         | Number of days employed (-ve values indicate current employment) |
| **EXT_SOURCE_1, 2, 3**    | Credit risk scores from external sources |
| **DAYS_CREDIT**           | Number of days since last credit inquiry |
| **CREDIT_UTILIZATION**    | Ratio of credit used to total credit limit |
| **AGE**                   | Borrower’s age |
| **NUMBER_OF_DEPENDENTS**  | Number of dependents in family |
| **PREVIOUS_LOANS_STATUS** | Historical repayment behavior |
| **LOAN_TYPE**             | Mortgage, Personal, Business, etc. |

These features help build a **predictive model** to assess loan repayment risk.

---

## 🔹 Project Workflow

### 1️⃣ Data Preprocessing & Feature Engineering
- Handle **missing values** in credit history & income data.
- **Feature scaling** using `MinMaxScaler` / `StandardScaler`.
- Convert categorical features using **Label Encoding**.
- Create new features: **Debt-to-Income Ratio, Loan-to-Value Ratio, etc.**.

---

### 2️⃣ Machine Learning Model Training

💡 **Selected Algorithms:**
✅ **Logistic Regression** – Baseline Model  
✅ **Random Forest / XGBoost** – Boosted Tree-based models for better accuracy  
✅ **Neural Networks (PyTorch / TensorFlow)** – Deep Learning for complex patterns  

📈 **Performance Metrics Evaluated:**
- **AUC-ROC Curve** (Measures classification performance).
- **Precision-Recall** (For handling class imbalance).
- **F1 Score** (Balances precision & recall).

---

### 3️⃣ Model Deployment (FastAPI & Docker)

📌 **Steps for Deployment:**
✅ **Train & save the model** as a `.pkl` or `.onnx` file.  
✅ **Build a FastAPI service** to expose model predictions.  
✅ **Deploy the API on AWS / GCP / Heroku** using **Docker & Kubernetes**.  
✅ **Connect a React.js dashboard** for real-time loan risk analysis.  

---

## 🔹 Expected Impact of the System
✅ **Reduces loan default risks** for banks by 25%.  
✅ **Speeds up loan approval process** with automated risk assessment.  
✅ **Enhances fraud detection** using predictive analytics.  
✅ **Provides explainability** using SHAP values for regulatory compliance.  


