# -Credit-Default-Risk
# 🏦 Home Credit Default Risk - Credit Scoring Model

## 📌 Business Problem

Financial institutions need to assess the probability that a client will default on a loan.
Incorrect risk assessment can lead to significant financial losses.

This project aims to build a machine learning model to predict the probability of default using the Home Credit dataset.

The data comes from the Kaggle competition:
Home Credit Default Risk.

---

## 📊 Dataset

The dataset contains historical loan application data, including:

- Client demographic information
- Credit history
- Previous applications
- Installment payments
- Bureau credit data

Target variable:
- `TARGET = 1` → Client defaulted
- `TARGET = 0` → Client repaid loan

---

## 🧠 Project Pipeline

### 1️⃣ Data Cleaning
- Missing value treatment
- Outlier detection
- Feature consistency validation

### 2️⃣ Feature Engineering
- Aggregations from bureau and previous applications
- Ratio features (income/credit, annuity/income)
- Temporal features

### 3️⃣ Modeling
Models evaluated:
- Logistic Regression
- Random Forest
- Gradient Boosting

### 4️⃣ Evaluation

Main metric:
- ROC-AUC

Secondary metrics:
- Recall (focus on default detection)
- Precision
- F1-score

---

## 📈 Results

Best Model: Gradient Boosting  
ROC-AUC: XX  
Recall (Default Class): XX  

The model prioritizes recall to minimize false negatives (high-risk clients wrongly classified as safe).

---

## 🛠 Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib / Seaborn
- Jupyter Notebook

---

## 📂 Project Structure
├── data/
│ ├── raw/
│ ├── processed/
│ └── external/
├── notebooks/
├── src/
│ ├── data/
│ ├── features/
│ ├── models/
│ └── utils/
├── models/
│ └── saved_models/
├── tests/
├── config/
├── requirements.txt
└── README.md


---

## 🚀 How to Run

1. Clone repository
2. Create virtual environment:
   python -m venv venv
3. Activate environment
4. Install dependencies:
   pip install -r requirements.txt
5. Run notebooks or training scripts

---

## 🎯 Business Impact

A reliable credit scoring model allows financial institutions to:

- Reduce default rates
- Improve capital allocation
- Expand financial inclusion safely

---

## 👤 Author

Paulino Tamborini  
Data Scientist  
