# ❤️ Heart Disease Prediction using Machine Learning

## 📌 Project Overview

This project focuses on predicting the presence of heart disease using machine learning techniques based on patient medical data. The goal is to assist in early diagnosis and reduce the risk of severe health conditions.

---

## 🎯 Objective

* Analyze patient health data to identify important features
* Build and compare multiple machine learning models
* Evaluate models using performance metrics
* Select the best model for accurate prediction

---

## 📊 Dataset Information

* Total Records: 303
* Total Features: 14
* No missing values present
* Target Variable: `target` (0 = No Disease, 1 = Disease)

### Key Features:

* Age
* Sex
* Chest Pain Type (cp)
* Resting Blood Pressure (trestbps)
* Cholesterol (chol)
* Maximum Heart Rate (thalach)
* Exercise Induced Angina (exang)
* Oldpeak, Slope, CA, Thal

---

## 🔍 Exploratory Data Analysis (EDA)

* No missing values found in dataset
* Data contains slight skewness in features like cholesterol and oldpeak
* Outliers observed but retained based on domain knowledge
* Correlation analysis shows:

  * **Chest Pain (cp)** and **Slope** strongly related to target

---

## ⚙️ Data Preprocessing

* Feature scaling applied using **StandardScaler**
* Train-Test Split: 70% training, 30% testing

---

## 🤖 Machine Learning Models Used

### 1. Logistic Regression

* Accuracy: **81%**
* ROC-AUC Score: **0.81**

---

### 2. Decision Tree Classifier

* Accuracy: **~74%**
* Improved using GridSearchCV
* Tuned Recall: **0.76**

---

### 3. Random Forest Classifier (Best Model ⭐)

* Accuracy: **~82%**
* ROC-AUC Score: **0.82**
* Recall Score: **0.84 → 0.86 (after tuning)**

---

## 📈 Model Evaluation Metrics

* Accuracy Score
* Precision, Recall, F1-score
* ROC-AUC Score
* Confusion Matrix

> ⚠️ In medical prediction, minimizing **false negatives** is critical.

---

## 🏆 Final Conclusion

* Random Forest performed best among all models
* High recall makes it suitable for medical diagnosis
* Model can help in early detection of heart disease

---

## 📊 Feature Importance

* Most important features include:

  * CA
  * Thal
  * Chest Pain (cp)
  * Thalach

---

## 📂 Project Structure

```bash
Heart-Disease-Prediction/
│── heart_disease_prediction.ipynb
│── heart.csv
│── README.md
│── requirements.txt
```

---

## ▶️ How to Run

```bash
pip install -r requirements.txt
jupyter notebook
```

---

## 🚀 Future Improvements

* Deploy using Streamlit or Flask
* Use Deep Learning models
* Add real-time patient data

---

## 🙌 Acknowledgements

* UCI Heart Disease Dataset
* Scikit-learn Documentation

---

## 📬 Contact

* GitHub: https://github.com/JayPatil-1119
* LinkedIn: www.linkedin.com/in/jay-patil-5b10422a7

---

⭐ If you like this project, give it a star!
