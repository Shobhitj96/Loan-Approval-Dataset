# Loan-Approval-Dataset

**Project Overview**

This project focuses on building a predictive model to assess loan approval risk based on applicant data. Using machine learning, the objective is to classify loan applicants as "risky" or "non-risky," supporting lenders in making data-driven decisions and minimizing financial risk.

**Dataset**

The dataset contains 252,000 records with various applicant characteristics, including:

Demographics: Marital status, gender, age

Financial Indicators: Income, job experience, home and car ownership

Location: City and state of residence

Target Variable: Risk_Flag — a binary indicator where 1 signifies a "risky" applicant and 0 signifies a "non-risky" one.

This data enables a thorough analysis of applicant profiles and provides a basis for effective risk prediction.

**Exploratory Data Analysis**

Initial exploration revealed trends such as varying default rates across states and certain professions. Visualizations like state-wise default rates helped uncover these insights, guiding feature selection and model preparation.

**Feature Engineering**

Key steps included:

1. Top Feature Selection: Using Random Forest, **the 10 most influential features were identified**, significantly associated with loan risk.

2. One-Hot Encoding: This step transformed categorical features into a numerical format, enabling accurate model training.

**Modeling Approach**

Model Selection and Evaluation

**Three main models were implemented: Logistic Regression, Random Forest, and XGBoost.** 

Here’s a summary of each model's performance:

Logistic Regression: Provided a solid baseline with 88% accuracy on the test set but struggled with identifying risky applicants due to imbalanced data, leading to a lower recall for the risky category.

Random Forest Classifier: Improved accuracy and showed better precision by capturing non-linear relationships; however, it still required further adjustment to improve recall for high-risk applicants.

XGBoost Classifier: This model achieved the highest accuracy of 89%, effectively balancing precision and recall by capturing more complex relationships within the data.

Ensemble Voting Classifier

To leverage the strengths of both Random Forest and XGBoost, an ensemble voting classifier was used. **This ensemble approach resulted in an accuracy of 89%, with enhanced recall for the risky class, balancing prediction strength across both categories.**

**Conclusion**

The combination of feature selection, rigorous model evaluation, and the final ensemble approach led to a model that offers substantial predictive power for loan risk assessment. This project demonstrated an increase in accuracy and recall, especially for high-risk applicants, providing valuable insights for lending decisions. The optimized XGBoost and ensemble models showcase how machine learning can effectively support risk management in financial services, enabling more confident and data-driven lending.






