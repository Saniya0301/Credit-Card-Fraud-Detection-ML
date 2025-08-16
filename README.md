# 💳 Credit Card Fraud Detection using Machine Learning

## 📌 Overview
This project implements **Credit Card Fraud Detection** using **Machine Learning techniques**. The dataset used contains transactions made by European cardholders in September 2013. The goal is to detect fraudulent transactions among credit card operations.

Due to the highly imbalanced nature of the dataset, different resampling techniques like **undersampling** and **SMOTE (oversampling)** are applied to improve classification performance.

---

## 📂 Dataset
- Dataset: [Credit Card Fraud Detection Dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud)  
- **Rows**: 284,807  
- **Features**: 30 (after preprocessing)  
- **Target variable**: `Class`  
  - `0` → Legitimate Transaction  
  - `1` → Fraudulent Transaction  

---

## ⚙️ Steps Performed
1. **Data Preprocessing**
   - Dropped `Time` column
   - Standardized `Amount` feature using `StandardScaler`
   - Removed duplicate entries

2. **Exploratory Data Analysis (EDA)**
   - Class distribution visualization using **Seaborn**

3. **Handling Imbalanced Data**
   - **Undersampling** → Reduced majority class  
   - **Oversampling with SMOTE** → Synthetic data generation  

4. **Model Training**
   - Logistic Regression  
   - Decision Tree Classifier  

5. **Evaluation Metrics**
   - Accuracy  
   - Precision  
   - Recall  
   - F1 Score  

6. **Model Saving**
   - Trained **Decision Tree Classifier** saved using `joblib` as `credit_card_model.pkl`

---

## 📊 Results

### Without Resampling
- **Logistic Regression**
  - Accuracy: `99.92%`
  - Precision: `0.88`
  - Recall: `0.60`
  - F1 Score: `0.71`

- **Decision Tree**
  - Accuracy: `99.90%`
  - Precision: `0.68`
  - Recall: `0.77`
  - F1 Score: `0.72`

---

### With Undersampling
- **Logistic Regression**
  - Accuracy: `92.6%`
  - Precision: `0.94`
  - Recall: `0.91`
  - F1 Score: `0.93`

- **Decision Tree**
  - Accuracy: `88.4%`
  - Precision: `0.89`
  - Recall: `0.89`
  - F1 Score: `0.89`

---

### With SMOTE (Oversampling)
- **Logistic Regression**
  - Accuracy: `94.38%`
  - Precision: `0.97`
  - Recall: `0.91`
  - F1 Score: `0.94`

- **Decision Tree**
  - Accuracy: `99.82%`
  - Precision: `0.99`
  - Recall: `0.99`
  - F1 Score: `0.99`

---
🛠️ Technologies Used

Python

Pandas, NumPy

Scikit-learn

Imbalanced-learn (SMOTE)

Seaborn, Matplotlib

Joblib


---
📜 License

This project is licensed under the MIT License.


