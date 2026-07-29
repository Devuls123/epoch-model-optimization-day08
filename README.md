# epoch-model-optimization-day08

# Customer Churn Model Optimization

**Name:** Devu L S  
**MUID:** lsdevu3@mulearn  

---

## Project Summary

This project focuses on improving customer churn prediction by comparing a baseline Decision Tree classifier with an optimized Random Forest classifier. The dataset was preprocessed by handling missing values, encoding categorical features, and preparing separate training and testing datasets. The optimized model was evaluated using Accuracy, Precision, Recall, and F1-Score to measure its predictive performance.

---

## Optimization Approach

The following optimization techniques were applied to improve the model performance:

- Removed missing values from the dataset.
- Converted categorical variables into numerical values using Label Encoding.
- Used the provided training dataset for model training and the testing dataset for evaluation.
- Built a **Decision Tree Classifier** as the baseline model.
- Improved the model using a **Random Forest Classifier** with optimized hyperparameters:
  - `n_estimators = 100`
  - `max_depth = 10`
  - `min_samples_split = 5`
- Compared the baseline and optimized models using multiple evaluation metrics.
- Performed feature importance analysis to identify the major factors influencing customer churn.

---

## Important Observations and Findings

Feature importance analysis showed that the following features had the greatest influence on customer churn:

| Feature | Importance |
|---------|-----------:|
| CustomerID | 0.632168 |
| Support Calls | 0.123023 |
| Total Spend | 0.085181 |
| Payment Delay | 0.054291 |
| Age | 0.051464 |

**Key Findings**

- The Random Forest model achieved better predictive performance than the Decision Tree baseline.
- **Support Calls** was the most important business-related factor influencing customer churn.
- **Total Spend** and **Payment Delay** also played significant roles in predicting customer churn.
- **Age** and **Contract Length** contributed moderately to the model.
- **CustomerID** received the highest importance score because it is a unique identifier. This feature should be removed before training future models, as it does not represent customer behavior and may lead to misleading feature importance.

---

## Model Improvements

Compared with the baseline Decision Tree model, the optimized Random Forest model provided:

- Improved prediction accuracy.
- Better Precision, Recall, and F1-Score.
- More stable and reliable predictions through ensemble learning.
- Better generalization on unseen test data.
- Feature importance analysis for understanding the factors affecting customer churn.

---

## Final Conclusion

The optimized Random Forest model successfully improved customer churn prediction compared to the baseline Decision Tree model. The analysis revealed that **Support Calls, Total Spend, Payment Delay, Age, and Contract Length** are the primary business factors influencing customer churn.

These insights can help organizations identify customers at risk of leaving and implement targeted retention strategies such as improving customer support, reducing payment issues, encouraging long-term contracts, and offering personalized retention programs.

Overall, the optimized model provides both accurate churn prediction and valuable business insights that support data-driven customer retention decisions.
