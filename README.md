# ml-project-credit-risk-model
# Credit Risk Modeling – Streamlit App

🔗 **Live App:** [https://credit-risk-model--ml-project.streamlit.app/](https://credit-risk-model--ml-project.streamlit.app/)

## 📌 Overview

This project is an end-to-end **Credit Risk Modeling** application built using **Machine Learning** and deployed with **Streamlit**. The app predicts the **probability of default**, generates a **credit score (300–900)**, and assigns a **credit rating** (Poor, Average, Good, Excellent) based on applicant and loan details.

The project demonstrates:

* Feature engineering for credit risk
* Logistic regression–based risk modeling
* Credit scorecard-style score transformation
* Interactive ML deployment using Streamlit

---

## 🚀 Features

* User-friendly Streamlit interface
* Real-time default probability prediction
* Credit score calculation mapped to industry-style ranges
* Risk rating categorization
* Scaled and preprocessed inputs using a saved pipeline

---

## 🧠 Model Details

* **Algorithm:** Logistic Regression
* **Target:** Probability of loan default
* **Scaling:** MinMaxScaler
* **Artifacts:** Stored using `joblib`

The model outputs:

* **Default Probability**
* **Credit Score (300–900)**
* **Rating:** Poor / Average / Good / Excellent

---

## 🗂️ Project Structure

```
├── main.py                  # Streamlit app
├── prediction_helper.py     # Model loading & prediction logic
├── artifacts/
│   └── model_data.joblib    # Trained model, scaler, features
├── requirements.txt         # Dependencies
├── README.md
```

---

## 📥 Input Parameters

The app takes the following inputs:

* Age
* Income
* Loan Amount
* Loan Tenure (months)
* Average DPD per delinquency
* Delinquency Ratio
* Credit Utilization Ratio
* Number of Open Loan Accounts
* Residence Type (Owned / Rented / Mortgage)
* Loan Purpose (Education / Home / Auto / Personal)
* Loan Type (Secured / Unsecured)

A **Loan-to-Income Ratio** is automatically calculated.

---

## 📊 Credit Score Logic

* Logistic regression output → Default Probability
* Non-default probability scaled to **300–900**
* Ratings:

  * **300–499:** Poor
  * **500–649:** Average
  * **650–749:** Good
  * **750–900:** Excellent

---

## 🛠️ Installation & Setup

### 1️⃣ Clone the repository

```bash
git clone https://github.com/your-username/credit-risk-model.git
cd credit-risk-model
```

### 2️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Run the Streamlit app

```bash
streamlit run main.py
```

---

## 📦 Requirements

Key libraries used:

* streamlit
* scikit-learn
* pandas
* numpy
* joblib
* xgboost

(See `requirements.txt` for exact versions)

---

## 🌐 Deployment

The app is deployed on **Streamlit Cloud**:
👉 [https://credit-risk-model--ml-project.streamlit.app/](https://credit-risk-model--ml-project.streamlit.app/)

---

## ⚠️ Disclaimer

This project is for **educational and demonstration purposes only**. It is **not** intended for real-world credit decisioning or regulatory use.

---

## 🙌 Acknowledgements

Inspired by real-world **credit scorecard modeling** and risk analytics practices in finance.

---

## 📬 Contact

If you’d like enhancements (SHAP explainability, XGBoost model, or API version), feel free to reach out.

