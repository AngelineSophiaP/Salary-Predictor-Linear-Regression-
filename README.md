# 📈 Salary Prediction Using Linear Regression

This project aims to predict employee salaries based on features such as Age, Gender, Education Level, and Years of Experience using a Linear Regression model in Python.

---

## 🧠 Objective

To build a predictive model that estimates an individual's salary using demographic and educational data, while exploring feature influence through correlation and regression analysis.

---

## 📁 Dataset Overview

The dataset contains the following key columns:

- `Age`
- `Gender` (Encoded as: Male = 0, Female = 1)
- `Education Level` (Encoded as:  
  - High School = 0  
  - Bachelor's = 1  
  - Master's = 2  
  - PhD = 3)
- `Years of Experience`
- `Salary` (Target variable)

---

## 🧹 Data Preprocessing

- Handled missing (`NaN`) values using mapping and `.dropna()`.
- Encoded categorical features using manual mapping and one-hot encoding.
- Cleaned column names and ensured numeric data types.
- Explored feature correlation with the salary.

---

## 📊 Correlation Analysis

| Feature               | Correlation with Salary |
|-----------------------|--------------------------|
| Age                  | -0.70                    |
| Gender               | -0.10                    |
| Education Level      | +0.40                    |
| Years of Experience  | +0.80                    |
| Job Title (encoded)  | ~0.00                    |

> 🔍 Observation: Years of experience and age have the strongest impact on salary prediction.

---

## 📘 Model: Linear Regression

- Model used: `sklearn.linear_model.LinearRegression`
- Training performed on cleaned and encoded dataset.

### 📌 Regression Equation:
Salary = 134081.86
- 2963.99 × Age
+ 7957.50 × Experience
+ 17443.70 × Education_Level
- 8087.09 × Gender

- 
---

## 📈 Evaluation Metrics

- **R² Score**: `0.64`  
  → Model explains 64% of salary variance.
- **MSE**: `1219551563`  
- **RMSE**: `~₹34,918`

---

## 🧪 Technologies Used

- Python (Pandas, NumPy, Scikit-learn)
- Data Visualization: Matplotlib, Seaborn
- Jupyter Notebook

---

## ✅ Conclusion

- Years of Experience is the most influential feature.
- Education level has a moderate positive impact.
- Gender and age showed weak or negative correlation.
- The model gives reasonably good predictions and can be improved further by adding more features such as job title, location, or company size.

---

## 🚀 Future Work

- Add job titles with proper encoding.
- Explore non-linear models (e.g., Random Forest, XGBoost).
- Use GridSearchCV for hyperparameter tuning.
- Deploy as a simple web app using Streamlit or Flask.

---



