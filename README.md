# 📊 Customer Churn Prediction using Artificial Neural Networks (ANN)

Customer churn is a critical problem in the banking industry. This project predicts whether a customer will leave the bank using an **Artificial Neural Network (ANN)** trained on demographic, financial, and behavioral customer data.

---

## 📌 Project Overview

The goal of this project is to build a deep learning model that accurately classifies bank customers as **churned** or **retained**. The model uses historical customer data and applies preprocessing, feature encoding, and neural network training to achieve reliable predictions.

---

## 📁 Dataset Information

- **File:** `Churn_Modelling.csv`
- **Records:** 10,000 customers
- **Target Variable:** `Exited`
  - `1` → Customer churned
  - `0` → Customer retained

### 🔑 Features
| Feature | Description |
|------|------------|
| CreditScore | Customer credit score |
| Geography | Customer country |
| Gender | Male / Female |
| Age | Customer age |
| Tenure | Years with the bank |
| Balance | Account balance |
| NumOfProducts | Number of bank products |
| HasCrCard | Credit card ownership |
| IsActiveMember | Active status |
| EstimatedSalary | Estimated annual salary |

---

## 🧠 Model & Methodology

### 1️⃣ Data Preprocessing
- Removed non-informative columns:
  - `RowNumber`, `CustomerId`, `Surname`
- Encoded categorical variables:
  - One-Hot Encoding for `Geography`
  - Binary Encoding for `Gender`
- Feature scaling applied for ANN optimization
- Train-test split:
  - **80% Training**
  - **20% Testing**

---

### 2️⃣ ANN Architecture
- Input Layer
- Hidden Layers with **ReLU activation**
- Output Layer with **Sigmoid activation**

**Loss Function:** Binary Crossentropy  
**Optimizer:** Adam  
**Metric:** Accuracy

---

## 📈 Model Training & Evaluation

- Trained over multiple epochs
- Validation split used to monitor overfitting
- Accuracy evaluated on unseen test data
- Training and validation accuracy curves plotted

📌 The model shows strong generalization performance without significant overfitting.

---

## 📊 Visualizations
- Dataset preview
- Training vs Validation Accuracy curve
- Model evaluation metrics

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- TensorFlow / Keras
- Matplotlib

---

## 📂 Project Structure

```text
Customer-Churn-Prediction/
│
├── Churn_Modelling.csv
├── Churn Modelling pred.ipynb
├── README.md
