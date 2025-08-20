# Credit Default Prediction  

## 📌 Overview  
This repository implements a **credit default classification system** based on financial and demographic data. The goal is to predict whether a credit card holder will **default on their next payment**, using information such as repayment history, credit utilization, and demographic variables.  

The project explores multiple machine learning models, comparing their predictive performance with respect to accuracy, out-of-sample error, and robustness.  

---

## 📂 Repository Structure  

```
├── db_default_data_creditcardsclients.csv
├── s_default_probabilities.ipynb
```

---

## 📊 Dataset  

The dataset contains information on **30,000 credit card clients** with the following features:  

- **Continuous variables**:  
  - Credit amount  
  - Bill amounts (for past 6 months)  
  - Payments made (for past 6 months)  
  - Age  

- **Categorical variables**:  
  - Gender  
  - Education  
  - Marital status  
  - Repayment status (coded from on-time payment to months of delay)  

🎯 **Target variable:** Default on next payment (Yes/No).  

---

## ⚙️ Methodology  

The workflow consists of:  

1. **Data Preparation**  
   - Data cleaning & standardization  
   - Training/testing split & scenario generation  

2. **Model Training**  
   - Logistic Regression variations  
   - CART (decision trees)  
   - Gradient Boosting  

3. **Evaluation**  
   - Out-of-sample error  
   - ROC curve and AUC  
   - Cross-validation  
   - Backtesting  

---

## 📈 Results Summary  

- **Logistic regression** provided a strong and interpretable baseline.  
- **Interaction terms and categorical variables** significantly improved performance.  
- **Regularization (Lasso)** enhanced model robustness and generalization.  
- **Tree-based methods (CART)** were less effective on this dataset.  
- **Boosting** offered competitive results, but was outperformed by enhanced logistic regression.  

👉 Overall, **regularized logistic regression with interactions and categorical variables** was the most effective model.  

---
