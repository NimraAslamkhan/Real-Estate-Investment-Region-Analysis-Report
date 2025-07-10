# Real-Estate-Investment-Region-Analysis-Report
# 🏡 Real Estate Investment Opportunity Prediction Report

## 📌 Project Title: Strategic Land Investment Analysis using Machine Learning

---

## 🧾 Problem Statement
The Land Rental Division seeks to optimize real estate investments by identifying high-potential properties based on location, size, price, and predicted returns. The primary objective is to build a machine learning pipeline that analyzes listings and recommends the **top 50 most profitable properties**.

---

## 🗂️ Step-by-Step Project Workflow

### 1️⃣ Data Collection & Loading
- Source File: `Melbrin_cleaned_data.csv`
- Data was loaded into a Pandas DataFrame.
- Initial shape and summary statistics were explored.

### 2️⃣ Data Preprocessing
- Handled missing values using **KNN Imputer**.
- Treated outliers using IQR and capping methods.
- Encoded categorical variables (e.g., region names using one-hot encoding).
- Normalized numerical features.

### 3️⃣ Model Training & Evaluation
- **10 machine learning models** were trained using cross-validation:
    - Logistic Regression
    - Random Forest
    - Gradient Boosting
    - Decision Tree
    - K-Nearest Neighbors (KNN)
    - Support Vector Machine (SVM)
    - Naive Bayes
    - XGBoost
    - AdaBoost
    - LightGBM

- **Performance Metrics Evaluated**:
    - Accuracy
    - F1 Score
    - Precision & Recall
    - AUC Score

### 🔍 Visualization: Model Comparison
- A bar chart was created comparing models based on F1 Score and Accuracy.
- **Best performing model: Random Forest** (based on high F1 and Accuracy).

### 4️⃣ Final Model Selection
- The **Random Forest** model was selected for final prediction.
- Confusion matrix and classification report were plotted.
- Predicted labels and probabilities were appended to the dataset.

### 5️⃣ Investment Filtering Logic
- Applied thresholding to find **top 25% building area** and **bottom 25% price**.
- Filtered listings predicted as “Good Investment” using the final model.
- Focused on **Western** and **South-Eastern Metropolitan** regions.
- Final shortlisting of **top 50 properties** based on predicted probabilities.

### 6️⃣ Region-Based Insights
- Extracted and summarized which **regions dominated the top 50 picks**.
- Bar plot generated for region distribution.
- Histogram plotted for predicted investment probabilities.

---

## 📈 Visualizations Included:
- ✅ Bar chart: Model performance comparison
- ✅ Confusion Matrix: Final model validation
- ✅ Classification Report: Precision, Recall, F1-score per class
- ✅ Bar chart: Top 50 properties by Region
- ✅ Histogram: Predicted investment confidence distribution

---



## ✅ Final Outcome & Recommendation

- The ML pipeline successfully identified top 50 real estate listings with the highest investment potential.
- These listings were large-area, low-price properties located mainly in **Western** and **South-Eastern Metropolitan** regions.
- The model’s predictions showed strong confidence (avg. prob > 0.8).
- **Recommendation**: Present these listings to stakeholders as prime investment targets.

---



