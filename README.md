# 💳 Credit Card Fraud Detection

This project uses a **Random Forest Classifier** to detect fraudulent credit card transactions using the **Credit Card Fraud Detection dataset** from Kaggle.

---

## 📌 Problem Statement

Credit card fraud is a significant challenge for banks and financial institutions. The goal of this project is to build a simple yet effective machine learning model to classify whether a transaction is **fraudulent (1)** or **legitimate (0)**.

---

## 📌 Dataset

- **Source:** [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud)
- **Records:** 284,807 transactions
- **Fraud cases:** Only ~0.17% are fraudulent (highly imbalanced dataset)
- Features: Time, Amount, V1–V28 (PCA-transformed for confidentiality)

---

## 📌 Workflow

1️⃣ **Data Loading:**  
Load the dataset and check class distribution.

2️⃣ **Data Preprocessing:**  
- Scale `Amount` and `Time` features using `StandardScaler`.

3️⃣ **Train-Test Split:**  
- Split data into training and testing sets (80/20).
- Use `stratify` to maintain class imbalance ratio.

4️⃣ **Model Training:**  
- Train a `RandomForestClassifier` with 100 trees.

5️⃣ **Model Evaluation:**  
- Evaluate model performance using accuracy score.

---

## 📌 Libraries Used

- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `seaborn`

---

## 📌 How to Run

1️⃣ Clone this repository:  
```bash
git clone https://github.com/yourusername/credit-card-fraud-detection.git
cd credit-card-fraud-detection

2️⃣ Install dependencies:

pip install pandas numpy scikit-learn matplotlib seaborn

3️⃣ Download the dataset from Kaggle and place creditcard.csv in the project folder.

4️⃣ Run the script:

python your_script_name.py
