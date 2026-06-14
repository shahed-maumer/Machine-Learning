# 📊 Machine Learning Assignment 2  
## Customer Personality Analysis

---

## 👩‍💻 Student Information
- Name: [shahed Muammer]
[ID:[2320224113
- Course: Machine Learning
- Assignment: 2

---

## 📌 Project Overview

This project applies Machine Learning techniques on the **Customer Personality Analysis dataset** to analyze customer behavior and build predictive models.

The project includes:
- Data Preprocessing
- Feature Engineering
- Supervised Learning (Regression & Classification)
- Unsupervised Learning (Clustering)

---

## 📂 Dataset

- Source: Kaggle - Customer Personality Analysis  
- File: `marketing_campaign.csv`

The dataset contains customer information such as:
- Income
- Year of Birth
- Spending on different product categories
- Family information
- Campaign responses

---

## 🧹 Data Preprocessing

The following steps were performed:

- Handled missing values in **Income** using median imputation  
- Removed unrealistic ages (<18 or >100)  
- Removed invalid income values (Income ≤ 0)  
- Encoded categorical variables:
  - Education → Label Encoding  
  - Marital Status → One-Hot Encoding (Top categories + Other)

---

## 🔧 Feature Engineering

New features were created:

- **Age** = Current Year - Year_Birth  
- **TotalSpending** = Sum of all product purchases  
- **TotalChildren** = Kidhome + Teenhome  

---

## 📈 Regression Task

### 🎯 Goal:
Predict **TotalSpending**

### Models Used:
- Linear Regression  
- Ridge Regression  
- Decision Tree Regressor  

### Evaluation Metrics:
- Mean Squared Error (MSE)  
- Root Mean Squared Error (RMSE)  
- R² Score  

---

## 🧠 Classification Task

### 🎯 Goal:
Predict customer response to marketing campaigns

### Models Used:
- Logistic Regression (class_weight='balanced')  
- K-Nearest Neighbors (KNN)  
- Random Forest Classifier  

### Evaluation Metrics:
- Accuracy  
- Precision  
- Recall  
- F1-Score  
- Confusion Matrix  

### ⚠️ Note:
Due to class imbalance, **Recall and F1-score are more important than Accuracy**.

---

## 📊 Clustering Task

### 🎯 Goal:
Customer Segmentation

### Features Used:
- Income  
- TotalSpending  
- Age  
- TotalChildren  

### Methods:
- K-Means Clustering  
- Elbow Method (optimal K selection)  
- PCA Visualization  

---

## 📉 Results & Insights

- Customers were successfully segmented into meaningful groups based on behavior.  
- Regression models predicted customer spending with reasonable accuracy.  
- Classification models identified likely responders to campaigns.  
- Clustering helped discover high-value customer segments.

---

## 🛠️ Technologies Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  

---

## 🚀 How to Run the Project

1. Upload `marketing_campaign.csv` in Google Colab  
2. Run the notebook step by step  
3. Ensure all required libraries are installed  
4. View results and visualizations  
