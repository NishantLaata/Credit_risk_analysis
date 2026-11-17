Project 01: Credit Risk Intelligence System

End-to-End Machine Learning and AI Project

1. Business Background

You are working as a Data Scientist at a credit card company. The company wants to improve its ability to identify customers who are likely to default on their credit card payments.

The company has historical customer data containing demographic information, credit limits, repayment history, bill amounts, and previous payment amounts.

The objective is to analyze historical customer behavior and develop a machine learning system that predicts the probability of a customer defaulting on their payment in the following month.

The business wants to use these predictions to improve risk assessment, identify potentially risky customers, and support better credit risk management decisions.

2. Main Business Problem Statement

How can we use historical customer financial behavior, repayment patterns, and demographic information to predict whether a credit card customer will default on their payment next month?

The system should estimate the probability of default for each customer and classify customers into different risk categories.

⸻

PART A: Exploratory Data Analysis (EDA)

Problem 1: Customer Demographics Analysis

Objective: Understand the demographic characteristics of customers and identify potential relationships between customer demographics and payment defaults.

Questions to investigate:

1. What is the age distribution of customers?
2. Which age groups have the highest number of customers?
3. Is there a relationship between customer age and payment default?
4. Does gender appear to have an association with default rates?
5. Which demographic segments have the highest default percentages?

Expected output:

* Age distribution visualization.
* Gender distribution.
* Default rate by age group.
* Default rate by gender.

Problem 2: Credit Limit Analysis

Objective: Understand how credit limits relate to customer repayment behavior and default risk.

Questions to investigate:

1. What is the average credit limit across all customers?
2. What is the distribution of customer credit limits?
3. Do customers with lower credit limits default more frequently?
4. Does having a higher credit limit necessarily indicate lower credit risk?
5. Which credit limit segments have the highest default rates?

Expected output:

* Credit limit distribution.
* Average credit limit by default status.
* Default rate across credit limit segments.
* Correlation between credit limit and default.

Problem 3: Repayment Behavior Analysis

Objective: Identify whether historical repayment behavior can help predict future customer defaults.

Questions to investigate:

1. Do customers who repeatedly delay payments have a higher probability of default?
2. Does a history of missed payments predict future default?
3. Which repayment month provides the strongest predictive signal?
4. Are customers with consistent repayment histories less likely to default?
5. How does the number of delayed payments relate to default probability?

Expected output:

* Repayment status distribution.
* Default rate by repayment status.

* Monthly repayment behavior analysis.
* Comparison of repayment patterns between defaulting and non-defaulting customers.

⸻

PART B: Financial Behavior Analysis

Problem 4: Bill Amount vs Payment Amount Analysis

Objective: Understand customer spending and repayment patterns by comparing outstanding bill amounts with actual payment amounts.

Questions to investigate:

1. What are the average monthly bill amounts?
2. Are customers paying their full outstanding balances?
3. What percentage of customers consistently pay less than their bill amount?
4. Does the difference between bill amount and payment amount correlate with default?
5. Are customers with consistently high outstanding balances more likely to default?

Expected output:

* Monthly bill amount distribution.
* Monthly payment amount distribution.
* Bill-to-payment ratio analysis.
* Default rate by payment behavior.

Problem 5: Payment Pattern Analysis

Objective: Identify customers whose payment behavior indicates increasing financial stress.

Questions to investigate:

1. Do customers who consistently make smaller payments have higher default rates?
2. Are there differences between customers who pay on time and those who delay?
3. Can we identify customers whose payment behavior is deteriorating?
4. Does increasing outstanding debt indicate a higher probability of default?
5. Which combination of payment behaviors is most strongly associated with default?

Expected output:

* Customer payment behavior segmentation.
* Payment trend analysis.
* Identification of potentially risky payment patterns.
* Default rate by payment behavior segment.

⸻

PART C: Machine Learning and Predictive Modeling

Problem 6: Credit Default Prediction

Objective: Develop machine learning models that predict whether a customer will default on their credit card payment next month.

Target variable:

default.payment.next.month

Target classification:

* 0 = No default
* 1 = Default

Tasks:

1. Prepare the dataset for machine learning.
2. Separate independent variables and the target variable.
3. Perform appropriate categorical variable encoding.
4. Split the dataset into training and testing sets.
5. Handle class imbalance if necessary.
6. Train a Logistic Regression model as the baseline.
7. Train an advanced model using XGBoost.
8. Compare the predictive performance of both models.

Expected output:

* Trained classification models.
* Predicted default probabilities.
* Comparison of model performance.
* Identification of the better-performing model.

Problem 7: Model Evaluation and Optimization

Objective: Evaluate the performance of machine learning models and determine whether they can reliably identify customers who are likely to default.

Evaluation metrics:

1. Accuracy
2. Precision
3. Recall
4. F1-score
5. ROC-AUC
6. Confusion Matrix
7. Precision-Recall Curve

Business questions:

1. How many actual defaulters can the model correctly identify?
2. How many reliable customers are incorrectly classified as high risk?
3. Which model performs better at identifying potential defaulters?
4. What is the trade-off between precision and recall?
5. Can model performance be improved through hyperparameter tuning?
6. What classification threshold provides an appropriate balance between business costs?

Expected output:

* Model evaluation report.
* Confusion matrices.
* ROC and precision-recall curves.
* Model comparison.
* Optimized classification threshold.

⸻

PART D: Explainable AI (XAI)

Problem 8: Understanding Model Predictions Using SHAP

Objective: Make machine learning predictions interpretable by identifying the factors influencing customer default risk.

Use SHAP (SHapley Additive exPlanations) to understand model behavior.

Questions to investigate:

1. Which features have the greatest influence on default predictions?
2. Does repayment history matter more than customer age?
3. How does credit limit influence predicted default risk?
4. Which financial behaviors increase the probability of default?
5. Why did a particular customer receive a high-risk prediction?
6. Are there any unexpected relationships identified by the model?

Expected output:

* Global feature importance.
* SHAP summary plot.
* SHAP dependence plots.
* Individual customer prediction explanations.
* Explanation of the most influential risk factors.

⸻

PART E: AI Engineering and Application Development

Problem 9: Build an AI-Powered Credit Risk Assistant

Objective: Develop an AI assistant that explains machine learning predictions in natural language.

Imagine a credit risk analyst asks:

“Why is Customer 102 classified as high risk?”

The AI assistant should:

1. Retrieve the customer’s actual model prediction.
2. Access the customer’s relevant financial features.
3. Retrieve the corresponding SHAP explanations.
4. Explain the most important factors contributing to the prediction.
5. Present the explanation in simple business language.
6. Answer follow-up questions about the customer’s risk profile.

Example response:

“Customer 102 has been classified as high risk based on the model’s prediction. The main contributing factors include repeated payment delays, relatively low recent payment amounts compared with outstanding bills, and a history of repayment difficulties.”

The AI assistant must use actual model outputs and feature explanations rather than inventing reasons.

Problem 10: Develop an Interactive Credit Risk Dashboard

Objective: Build an interactive application using Streamlit that allows business users and credit risk analysts to explore customer risk predictions.

The dashboard should include:

1. Total number of customers analyzed.
2. Overall customer default rate.
3. Distribution of customers across risk categories.
4. Important factors influencing default predictions.
5. Individual customer risk prediction.
6. Predicted probability of default.
7. Individual customer SHAP explanation.
8. AI-powered natural language explanation.
9. Interactive customer filtering and exploration.

Expected output:

* Interactive Streamlit dashboard.
* Customer risk classification.
* Individual prediction interface.
* AI-powered risk explanation.
* Model performance visualization.

⸻

3. Final Project Deliverables

By the end of this project, the following components should be completed:

1. Real-world credit card customer dataset.
2. Exploratory Data Analysis report.
3. Data cleaning and feature engineering pipeline.
4. SQL-based analytical queries.
5. Logistic Regression classification model.
6. XGBoost classification model.
7. Model evaluation and comparison report.
8. SHAP-based explainable AI implementation.
9. AI-powered Credit Risk Assistant.
10. Interactive Streamlit dashboard.
11. GitHub repository with documentation.
12. Project README explaining the business problem, methodology, results, and limitations.

⸻

4. Overall Project Objective

The ultimate goal is to develop an end-to-end Credit Risk Intelligence System that combines traditional data science, predictive machine learning, explainable AI, and generative AI.

The final solution should demonstrate the ability to:

* Analyze real-world financial data.
* Extract meaningful business insights.
* Develop and evaluate predictive machine learning models.
* Explain model predictions.
* Integrate generative AI with machine learning outputs.
* Develop an interactive application.
* Translate machine learning results into actionable business intelligence.

Important: This system is intended to support credit risk analysis, not automatically approve or reject customers. Model performance, fairness, data limitations, and business costs must be evaluated before any real-world deployment.
