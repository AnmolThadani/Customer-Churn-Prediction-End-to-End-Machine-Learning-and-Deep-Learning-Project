# Customer Churn Prediction: End-to-End Machine Learning and Deep Learning Project

🎯 **Objective**:  
This project focuses on predicting customer churn using a telecom dataset. It involves comprehensive **data cleaning**, **exploratory data analysis (EDA)**, and implementation of **machine learning models**, **deep learning models**, and **visualizations** to extract insights and deliver actionable results.

---

## 📖 **Project Overview**

Customer churn is a critical business problem for subscription-based companies like telecom providers. This project aims to predict whether a customer will churn (leave the company) based on their subscription and usage data. By identifying factors contributing to churn, businesses can implement targeted retention strategies to reduce customer attrition.

---

## 📊 **Dataset Details**

The dataset used in this project is the **Telco Customer Churn** dataset. It contains demographic, account, and usage information for 7,043 customers. The target variable, `Churn`, indicates whether a customer has churned (`Yes`) or not (`No`).

### **Features:**
- **Customer Demographics**: `Gender`, `SeniorCitizen`, `Partner`, `Dependents`
- **Account Information**: `Contract`, `PaperlessBilling`, `PaymentMethod`
- **Service Details**: `PhoneService`, `InternetService`, `OnlineSecurity`, etc.
- **Usage Metrics**: `MonthlyCharges`, `TotalCharges`, `tenure`

---

## ⚙️ **Workflow**

The notebook is structured as follows:

1. **Data Cleaning**:
   - Handle missing values and inconsistent data types.
   - Standardize categorical values.

2. **Feature Engineering**:
   - Create new features like `tenure_bins`.
   - Apply one-hot encoding to categorical columns.
   - Normalize numerical features.

3. **EDA (Exploratory Data Analysis)**:
   - Analyze churn distribution and correlations.
   - Visualize relationships between features and churn.

4. **Machine Learning Models**:
   - Logistic Regression
   - Random Forest
   - XGBoost

5. **Deep Learning**:
   - A fully connected neural network with dropout layers.

6. **Model Evaluation**:
   - Confusion matrix, accuracy, precision, recall, F1-score.
   - ROC-AUC curve for performance comparison.

---

## 🧠 **Machine Learning Models**

### **1. Logistic Regression**
- Baseline model for churn prediction.
- Quickly identifies the influence of each feature on churn.

### **2. Random Forest**
- Captures non-linear relationships in the data.
- Provides feature importance rankings.

### **3. XGBoost**
- Gradient boosting model for high-performance churn prediction.
- Handles imbalanced data effectively.

---

## 🤖 **Deep Learning Model**

### **Architecture**:
- **Input Layer**: Accepts all customer features.
- **Hidden Layers**:
  - 1st Layer: 64 neurons, ReLU activation, 30% dropout.
  - 2nd Layer: 32 neurons, ReLU activation, 30% dropout.
- **Output Layer**: 1 neuron with sigmoid activation.
- **Optimizer**: Adam
- **Loss Function**: Binary Cross-Entropy

---

## 📈 **Results**

### **Model Performance:**

| Model               | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|---------------------|----------|-----------|--------|----------|---------|
| Logistic Regression | 80.2%   | 78.5%     | 65.3%  | 71.3%    | 0.84    |
| Random Forest       | 83.5%   | 81.2%     | 71.8%  | 76.2%    | 0.88    |
| XGBoost             | 85.4%   | 83.1%     | 74.5%  | 78.6%    | 0.90    |
| Deep Learning       | 86.1%   | 84.5%     | 75.9%  | 79.9%    | 0.91    |

- **Best Model**: Deep Learning with an accuracy of **86.1%** and an ROC-AUC of **0.91**.

---
