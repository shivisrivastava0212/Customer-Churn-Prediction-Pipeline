# 🚀 Telco Customer Churn Prediction

A production-ready Machine Learning project for predicting customer churn using Logistic Regression and structured evaluation metrics.

---

# 📌 Table of Contents

1. Project Overview
2. Problem Statement
3. Dataset Information
4. Project Workflow
5. Tech Stack
6. Installation & Setup
7. Running the Project
8. Model Training
9. Hyperparameter Tuning
10. Results & Evaluation
11. Model Files
12. Deployment
13. Future Improvements
14. Author

---

# 1️⃣ Project Overview

Customer churn prediction helps businesses identify customers who are likely to leave.
This project builds a machine learning pipeline to predict churn using customer behavior and service usage data.

**Goal:**
Predict whether a customer will churn or not.

---

# 2️⃣ Problem Statement

Telecom companies lose revenue when customers leave. By predicting churn early, businesses can take preventive actions.

**Target Variable:**
`Churn`

---

# 3️⃣ Dataset Information

Dataset used:
`Telco_customer_churn.xlsx`

### Features include:

* Gender
* SeniorCitizen
* Contract Type
* Monthly Charges
* Tenure
* Internet Service
* Payment Method
* etc.

---

# 4️⃣ Project Workflow

```text
Data Collection
      ↓
Data Cleaning
      ↓
EDA
      ↓
Feature Engineering
      ↓
Train-Test Split
      ↓
Model Training
      ↓
Evaluation
      ↓
Deployment
```

This structure helps readers understand the project in one go.

---

# 5️⃣ Tech Stack

* Python
* Jupyter Notebook
* Google Colab
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn

---

# 6️⃣ Installation & Setup

## Option 1: Run on Google Colab (Recommended)

1. Open Google Colab.
2. Upload `Logestic_Regression.ipynb`
3. Upload dataset file.
4. Click **Runtime → Run All**.

## Option 2: Run Locally

Clone repository:

```bash
git clone <your-repo-link>
cd <repo-name>
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Launch notebook:

```bash
jupyter notebook
```

---

# 7️⃣ Running the Project

Execute notebook cells sequentially:

```bash
Run Cell → Preprocessing
Run Cell → Training
Run Cell → Evaluation
Run Cell → Save Model
```

---

# 8️⃣ Model Training

Model used:

`Logistic Regression`

Training pipeline includes:

* Feature scaling
* Train-test split
* Model fitting
* Probability prediction

---

# 9️⃣ Hyperparameter Tuning

### Best Parameters Used

| Parameter | Value |
|-----------|-------|
| Solver | `lbfgs` |
| C | `1.0` |
| Max Iterations | `100` |
| Random State | `42` |
| Class Weight | `None` |

---

### Improved Balanced Model

| Parameter | Value |
|-----------|-------|
| Solver | `lbfgs` |
| C | `1.0` |
| Max Iterations | `1000` |
| Random State | `42` |
| Class Weight | `balanced` |

---

### Training Optimization

✅ Class imbalance handled using `class_weight='balanced'`  

✅ Increased iterations (`max_iter=1000`) for stable convergence  

✅ 5-Fold Cross Validation performed  

✅ Best trained model saved for deployment  

---

### Saved Model File

```python
best_model.pkl
```
# 🔟 Results & Visualizations

## Model Performance

| Metric | Score |
|--------|-------|
| Accuracy | 79.77% |
| Precision | 67.27% |
| Recall | 56.00% |
| F1 Score | 61.12% |
| ROC-AUC | 84.64% |

---

## Confusion Matrix

<img width="565" height="460" alt="confusion_matrix" src="https://github.com/user-attachments/assets/a93635ae-a64d-4786-aa16-ad21b48869b0" />

---

## ROC Curve

<img width="696" height="548" alt="roc_curve" src="https://github.com/user-attachments/assets/675fb6da-9487-49f6-af66-8e4530cea6a0" />


---

## Feature Coefficient Plot
<img width="645" height="442" alt="feature_coefficient" src="https://github.com/user-attachments/assets/a28d0e27-8303-49ed-83ae-090baee61b13" />





---




# 1️⃣1️⃣ Saved Model Files

```text
models/
```

```text
best_model.pkl
scaler.pkl
encoder.pkl
```

These files allow direct inference without retraining.

---

# 1️⃣2️⃣ Deployment

Possible deployment options:

## Streamlit

```bash
streamlit run app.py
```

## Flask

```bash
python app.py
```

## Docker

```bash
docker build -t churn-model .
docker run -p 8501:8501 churn-model
```

---

# 1️⃣3️⃣ Future Improvements

* Try XGBoost
* Try Random Forest
* Feature selection
* Handle class imbalance
* Model monitoring

---

# 1️⃣4️⃣ Repository Structure

```text
project/
│
├── data/
├── notebooks/
├── models/
├── results/
├── app/
├── requirements.txt
├── README.md
└── .gitignore
```

---

# 👩‍💻 Author

Shivi Srivastava

