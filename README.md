# Predicting customer churn in telecom. Using Data-Driven Insights to Improve Customer Retention

### Overview
**Data source:** [Telecom Churn](https://www.kaggle.com/datasets/shilongzhuang/telecom-customer-churn-by-maven-analytics/data)

- Customer churn is the percentage of customers who stop using a business's products or services over a specific period of time
- Customer churn can significantly impact revenue and growth. A proactive approach helps reduce turnover and maximize lifetime customer value.
- Data source contains information on all 7,043 customers from a Telecommunications company in California in Q2 2022 (37 features)
- Objective is to create a model to predict which customers are likely to churn

#### Proportion of Customer Status by Categorical Features
  <img width="666" alt="Screenshot 2024-10-28 at 1 39 14 AM" src="https://github.com/user-attachments/assets/9edf2ff7-d9a9-4876-9c6a-724065b7e82a">


#### Modeling Approach
- Classification allows us to predict churn (yes/no) for each customer.
- Models Tested: 
Decision Tree, Logistic Regression, Random Forest
- Final Model: 
Random Forest (higher accuracy and ROC AUC)


#### Evaluation Metrics
To evaluate the model’s effectiveness, we used several metrics tailored to understand how well it predicts churn.

1. Accuracy (82%) - Overall correctness of predictions
2. Recall (76%) - Ability to identify all customers likely to churn
3. ROC AUC (0.89) - model's ability to distinguish between churn and non-churn customers

The Random Forest model shows a slight advantage over Logistic Regression in terms of overall prediction accuracy (82% vs. 79%) and ROC AUC (0.89 vs. 0.88), indicating it’s more effective at distinguishing between churners and non-churners across thresholds. While Logistic Regression achieves a higher recall of 80% (compared to 76% for Random Forest), meaning it captures more actual churners, Random Forest balances this with a better precision of 64% for predicting churn, reducing false positives. This balance helps minimize misclassifications where non-churners are incorrectly flagged as likely to leave, which can save resources when targeting retention efforts.

In choosing a model, Random Forest stands out due to its overall higher accuracy and balanced performance between precision and recall, making it more reliable in capturing key churn patterns. Its ability to model complex relationships allows it to adapt better to the nuances of customer behavior, making it a stronger choice for prioritizing both accuracy and practical application in targeted retention strategies.


#### Top Feature Importance
1. Contract Type - month-to-month contracts increase churn risk;
2. Number of Referrals - more referrals associate with staying;
3. Total Charges - higher charges correlate with churn.


#### Recommendations
- Target high-risk segments focus on month-to-month customers;
- Offer incentives for longer contracts 
encourage commitment;
- Address high-charge dissatisfaction
offer tailored discounts or value-adds.
   
