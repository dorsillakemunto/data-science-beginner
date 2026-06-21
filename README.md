# Customer Churn Analysis 

## Project Overview 
In this project, I analyzed customer churn data to understand why customers leave a service and built machine learning models to predict churn. The goal was to identify the main factors driving churn and provide actionable insights to improve customer retention featuring an interactive Power BI dashboard.
![Power BI Dashboard Overview](Customer_Churn%20Overview-Dashboard.png)
## Key Findings 

### Customer Churn Rate 
* **Churn Rate:** 26.54% 
* **Retention Rate:** 73.46% 
![Churn Distribution](Customer_Churn%20Distribution.png)

*Insight: Approximately 1 in every 4 customers left the service, highlighting the importance of customer retention strategies.*

### Contract Type and Churn 
Contract type was one of the strongest factors affecting customer churn. 

| Contract Type | Stayed | Churned |
| :--- | :---: | :---: |
| **Month-to-Month** | 57% | 43% |
| **One Year** | 88% | 11% |
| **Two Year** | 97% | 2% |
![Contract Type vs Churn](Contract%20Type%20Vs%20Churn.png)

*Insight: Customers on month-to-month contracts were significantly more likely to churn, while customers on longer contracts showed much higher retention rates.*

### Monthly Charges and Churn 
* **Average Monthly Charges (Retained):** $61.26 
* **Average Monthly Charges (Churned):** $74.44 
![Monthly Charges vs Churn](Monthly%20Charges%20Vs%20Churn.png)


*Insight: Customers with higher monthly charges were more likely to leave the service.*

### Tenure and Churn 
* **Average Tenure (Retained):** 37.57 months 
* **Average Tenure (Churned):** 17.98 months 
![Tenure vs Churn](Tenure%20Vs%20Churn.png)

*Insight: Newer customers were more likely to churn, while long-term customers were more likely to remain loyal.*

### Customer Demographics and Churn 
The demographic analysis showed that gender had little to no influence on churn, with male and female customers displaying similar churn patterns. However, senior citizen status showed a noticeable relationship with churn: 

* **Non-Senior Customers:** ~4,000 stayed | ~1,400 churned. 
* **Senior Customers:** ~800 stayed | ~600 churned. 
![Demographics vs Churn](Demographics%20Vs%20Churn.png)

*Insight: Senior citizens had a higher tendency to churn compared to non-senior customers, suggesting an opportunity for targeted retention efforts.*

## Key Drivers of Churn 
The strongest variables associated with customer churn and most useful for predictive modeling:
* Internet Service 
* Payment Method 
* Monthly Charges 
* Paperless Billing 
* Senior Citizen Status 
* Streaming TV & Movies Subscriptions 
* Multiple Phone Lines 

## Machine Learning Results 

### Logistic Regression 
* **Accuracy:** 77.64% 
* **F1 Score:** 54.41% 
* **ROC-AUC Score:** 80.26% 

### Random Forest 
* **Accuracy:** 79.49% 
* **F1 Score:** 54.63% 
* **ROC-AUC Score:** 80.26% 

*Insight: The Random Forest model achieved the best overall performance, correctly predicting customer churn with nearly 80% accuracy.*

## Business Recommendations 
* **Contract Incentives:** Encourage customers to move from month-to-month contracts to longer-term plans. 
* **Onboarding Focus:** Focus retention efforts on new customers during their first few months of service. 
* **Pricing Reviews:** Review pricing strategies for customers with high monthly charges. 
* **Targeted Support:** Provide targeted support and engagement for senior customers. 
* **Proactive Engagement:** Use predictive models to identify and proactively engage customers at risk of churning. 

## Conclusion 
This project combined exploratory data analysis and machine learning to identify the factors driving customer churn. The analysis revealed that contract type, tenure, monthly charges, payment method, internet services, and senior citizen status were among the most important predictors of churn. The Random Forest model achieved nearly 80% accuracy, demonstrating how data-driven insights can help businesses identify at-risk customers and improve retention strategies.
