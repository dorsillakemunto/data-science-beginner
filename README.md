# Customer Churn Analysis 

## Project Overview 
In this project, I analyzed customer churn data to understand why customers leave a service and built machine learning models to predict churn. The goal was to identify the main factors driving churn and provide actionable insights to improve customer retention featuring an interactive Power BI dashboard.
![Customer Churn Overview Dashboard](Images/Customer%20Churn%20Overview%20Dashboard.png) 

## 🛠️ Tools & Technologies

- Python
- Google Colab
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Power BI
- GitHub

##  Dataset

This project uses the **Telco Customer Churn dataset**, which contains customer demographics, account information, services subscribed to, billing details, and churn status.

**Target Variable:** Churn (Yes/No)

##  Project Workflow

1. Data Collection
2. Data Cleaning and Preprocessing
3. Exploratory Data Analysis (EDA)
4. Feature Engineering
5. Model Building
6. Model Evaluation
7. Power BI Dashboard Creation
8. Business Insights and Recommendations

## Key Findings 

### Customer Churn Rate 
* **Churn Rate:** 26.54% (1,869 customers)
* **Retention Rate:** 73.46% (5,174 customers)
![Customer Churn Distribution](Images/Customer%20Churn%20Distribution.png)

*Insight: Approximately 1 in every 4 customers left the service, highlighting the importance of customer retention strategies.*

### Contract Type and Churn 
Contract type was one of the strongest factors affecting customer churn. 

| Contract Type | Stayed | Churned |
| :--- | :---: | :---: |
| **Month-to-Month** | 57% | 43% |
| **One Year** | 88% | 11% |
| **Two Year** | 97% | 2% |
![Contract Type Vs Churn](Images/Contract%20Type%20Vs%20Churn.png)

*Insight: Customers on month-to-month contracts were significantly more likely to churn, while customers on longer contracts showed much higher retention rates.*

### Monthly Charges and Churn 
* **Average Monthly Charges (Retained):** $61.26 
* **Average Monthly Charges (Churned):** $74.44 
![Monthly Charges Vs Churn](Images/Monthly%20Charges%20Vs%20Churn.png)


*Insight: Customers with higher monthly charges were more likely to leave the service.*

### Tenure and Churn 
* **Average Tenure (Retained):** 37.57 months 
* **Average Tenure (Churned):** 17.98 months 
![Tenure Vs Churn](Images/Tenure%20Vs%20Churn.png)

*Insight: Newer customers were more likely to churn, while long-term customers were more likely to remain loyal.*

### Customer Demographics and Churn 
The demographic analysis showed that gender had little to no influence on churn, with male and female customers displaying similar churn patterns. However, senior citizen status showed a noticeable relationship with churn: 

* **Non-Senior Customers:** ~4,000 stayed | ~1,400 churned. 
* **Senior Customers:** ~800 stayed | ~600 churned. 
![Demographics Vs Churn](Images/Demographics%20Vs%20Churn.png)

*Insight: Senior citizens had a higher tendency to churn compared to non-senior customers, suggesting an opportunity for targeted retention efforts.*

## Key Drivers of Churn

The machine learning model identified the top 15 variables driving customer churn. They can be broken down into three main categories:

* **Financials & Tenure (Strongest):** Total charges, monthly charges, and how long a customer has stayed (`tenure`) completely dominate the model's predictions.
* **Services & Billing Options (Moderate):** Using Fiber Optic internet, paying via Electronic Check, and contract terms play a major secondary role.
* **Demographics (Weakest):** Personal details like gender, being a senior citizen, or having dependents have the least predictive power on our list.

![Feature Importance](Images/Feature%20Importance.png)

##  Machine Learning Models

Two classification models were developed and evaluated to predict customer churn:

- Logistic Regression
- Random Forest Classifier

Both models were compared using multiple evaluation metrics to determine the best-performing model.


### Logistic Regression 
* **Accuracy:** 77.64% 
* **F1 Score:** 54.41% 
* **ROC-AUC Score:** 80.26% 

### Random Forest 
* **Accuracy:** 79.49% 
* **F1 Score:** 54.63% 
* **ROC-AUC Score:** 80.26% 

*Insight: The Random Forest model achieved the best overall performance, correctly predicting customer churn with nearly 80% accuracy.*

### Business Recommendations

* **Contract Incentives:** Encourage customers to move from month-to-month contracts to longer-term plans.
* **Onboarding Focus:** Focus retention efforts on new customers during their first few months of service to build tenure.
* **Pricing Reviews:** Review pricing strategies for customers with high monthly and total charges.
* **Targeted Support:** Provide targeted support and engagement for senior customers.
* **Proactive Engagement:** Use predictive models to identify and proactively engage customers at risk of churning.

## 📁 Repository Structure

Customer_Churn_Analysis/
│
├── Customer_Churn_Analysis.ipynb
├── README.md
├── Images/
│   ├── Customer Churn Overview Dashboard.png
│   ├── Customer Churn Distribution.png
│   ├── Contract Type Vs Churn.png
│   ├── Monthly Charges Vs Churn.png
│   ├── Tenure Vs Churn.png
│   ├── Demographics Vs Churn.png
│   └── Feature Importance.png


## Skills Demonstrated

- Data Cleaning and Preprocessing
- Exploratory Data Analysis (EDA)
- Data Visualization
- Feature Engineering
- Machine Learning Classification
- Model Evaluation and Comparison
- Business Insights Generation
- Power BI Dashboard Development

### Conclusion

This project combined exploratory data analysis, interactive Power BI visuals, and machine learning to identify the factors driving customer churn. The analysis revealed that total charges, tenure, monthly charges, payment method, contract type, internet services, and senior citizen status were among the most important predictors of churn. The Random Forest model achieved nearly 80% accuracy, demonstrating how data-driven insights can help businesses identify at-risk customers and improve retention strategies.

## Author

**Dorsilla Kemunto**

Aspiring Data Analyst passionate about using data to solve business problems and drive decision-making.

- GitHub: https://github.com/dorsillakemunto
- Email: dorsillakemunto@gmail.com

