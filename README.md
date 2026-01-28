# Customer Churn Analysis

**Author:** Manan Verma  
**Project Type:** Data Analysis and Machine Learning

## Project Overview
This project analyzes customer churn data to understand customer behavior and build predictive models. The analysis includes data exploration, filtering business conditions, and building regression models to study relationships between customer tenure, charges, and churn.

## Objective
- Analyze customer churn dataset
- Perform data quality checks
- Extract customers based on business rules
- Build regression models for prediction
- Evaluate model performance

## Dataset Description
- **Dataset contains:** Customer demographic, service, billing, and churn information
- **Total records:** 7043
- **Total features:** 21
- **Target variable for classification:** Churn

## Tools and Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Data Quality Checks
- ✅ **No missing values** found
- ✅ **No duplicate records** found
- ✅ **Data types verified** for all columns

## Analysis Performed

### 1. Business Rule Filtering
**Extracted customers who:**
- Have a **two-year contract**
- Use **mailed check** as payment method
- Have **churn value as "Yes"**

**Result stored for further analysis.**

### 2. Linear Regression
**Objective:** Predict `MonthlyCharges` using `tenure`

**Steps:**
- Train-test split in **70:30** ratio
- **Model:** Linear Regression
- **Evaluation metric:** Root Mean Squared Error (RMSE)

**Result:**  
**RMSE ≈ 29.08**

### 3. Logistic Regression (Single Variable)
**Objective:** Predict `Churn` using `MonthlyCharges`

**Steps:**
- Train-test split in **65:35** ratio
- **Model:** Logistic Regression
- **Evaluation metrics:** Confusion Matrix, Accuracy

**Result:**  
**Accuracy ≈ 72.87%**

### 4. Multiple Logistic Regression
**Objective:** Predict `Churn` using `tenure` and `MonthlyCharges`

**Steps:**
- Train-test split in **80:20** ratio
- **Model:** Logistic Regression
- **Evaluation metric:** Accuracy

**Result:**  
**Accuracy ≈ 79.77%**

## Key Insights
- **Tenure has a strong relationship** with customer charges
- **Monthly charges alone** provide moderate churn prediction
- **Combining tenure and monthly charges** improves churn prediction accuracy
- **Data quality plays a critical role** in reliable modeling
