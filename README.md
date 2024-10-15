# Exploratory Data Analysis - Churn Project

Cristiane Mecca Giacomazzi (Data Analyst)

This project was developed with Cross-industry standard process for data mining (CRISP-DM) methodology.
The following topics will be presented:
1. Business Understanding
2. Data Understanding
3. Ethical Statements
4. Data Preparation
5. Dictionary
6. Libraries used for this project
7. Project plan
8. Analysis  
  8.1 EDA
  8.2 Diagnostic
    8.2.1 Correlation 
9. Communication and Action
10. SWOT Analysis
--------------------------------------------------------------------------------------------------------
## 1. Business Understanding

  Churn represents the number of customers who end their relationship with a company within a specific period (Danao & Watts, 2024). This occurs when customers or subscribers stop engaging with your business. 
  As a key business metric, the churn rate is crucial for understanding customer behavior and loyalty, especially in a competitive market. Gaining this insight is vital for sustaining growth. Knowing your churn rate is essential for making decisions that enhance customer retention and loyalty. It allows you to assess your marketing strategy, the products you're offering, and, ultimately, predict your business's financial health. With this information, companies can adjust their strategies and refocus efforts to reduce churn.
  A higher churn rate signals that customers are leaving your business, resulting in lost clients. The “revenue churn rate” further highlights the percentage of revenue lost due to customer attrition, and both metrics are expressed as percentages.
  The importance of customer retention goes beyond loyalty; it's also cost-effective. Acquiring a new customer is five to 25 times more expensive than retaining an existing one (Gallo, 2014). Furthermore, Reichheld of Bain & Company (2021) found that increasing customer retention by just 5% can boost profits by 25% to 95%.
  Danao and Watts (2024) suggest that for mature and established companies, the ideal annual churn rate is between 5% and 7%, with a monthly churn rate of less than 1%. Nonetheless, the churn depend on the field of company. A 1% churn rate can represent millions of dollars in loss, hence it is necessary to understand the impact of churn on the business you are involved with (Truta, 2018).
  By actively monitoring churn rates, businesses can identify trends and areas for improvement, enabling them to implement targeted strategies to reduce customer loss and drive long-term success.
  The purpose of Part 1 of the project is to conduct exploratory data analysis on a public bank dataset, providing insights to identify customers with a higher likelihood of churning.

## 2. Data Understanding

Data Source: This project used a dataset from the Kaggle Website called “Churn_modelling” (https://www.kaggle.com/datasets/shubh0799/churn-modelling/data), a structured dataset.

Initial data exploration: Python, using Google Collab.

## 3. Ethical Statements

This project complies with the TCPS 2. The dataset is in the public domain.

## 4. Data Preparation

There is no missing or duplicated data in the dataset. However, outliers in the Age variable have been removed. Outliers were identified using the 1.5 times the interquartile range (IQR) rule. Additionally, the column containing surnames has been deleted.

## 5. Dictionary
<img width="565" alt="Screen Shot 2024-10-14 at 8 15 48 PM" src="https://github.com/user-attachments/assets/7b5e5049-7cb2-46aa-b7c9-87ae4c1988af">

## 6. Libraries used to project

Pandas, Matplotlib and Seaborn

## 7. Project Plan

  <img width="886" alt="Screen Shot 2024-10-14 at 8 17 42 PM" src="https://github.com/user-attachments/assets/70374089-f61b-42a1-8c68-395a25ac0b10">

## 8. Exploratory Analysis

The data were analyzed using the median and interquartile range (IQR) for numerical variables due to their asymmetry, while relative frequencies were employed to describe the categorical variables.

### Descriptive Analysis
- Churn represents 20.4% of the clients, which means a high percentage.
- Among the Germans, the customers have the highest churn rate (32%) versus 16% of Frenchies and Spanishies.
- Females also represent the higher percentage of churn with 25%, while Male represents 16%.
- Clients who consume 4 products in the bank have a 100% churn rate.
- 23% of the clients have been with the bank for 1 year.
- The churn rate of customers who have credit card is 20.81%, against 20.18% who do not have. This is an insignificant difference.
- 13% of inactive clients in the bank leave the bank.
- The median Credit Score is 646 points in the churn rate group, while in the no churn group the median is 653.
- The median of age is 44 years old in the churn rate group, higher then in no churn group (36 years old).
- The median of balance of clients who leave the bank is $109,163.42, higher then comparing to no churn group ($92,224.00)
- The median of estimated salary is $102,127.00 in the churn rate group, higher then comparade with no churn group ($99,800.00).

### Diagnostic Analysis - correlation
Considering the Pearson correlation, the relations between variables in general are the following:
- Balance x Age: r = 0.028 - positive and near zero relation
- Estimated Salary x Age: r = -0.0072 - negative and near zero relation
- Credit Score x Age: r = -0.004 - negative and near zero relation
- Balance x Estimated Salary: r = 0.013 - positive and near zero relation
- Balance x Credit Score: r = 0.0063 - positive and near zero relation
- Estimated Salary x Credit Score: r = -0.0014 - negative and near zero relation
  
When analyzing just the churn group, the relations seem the same:
- Balance x Age: r = 0.023 - positive and near zero relation
- Estimated Salary x Age: r = -0.0011 - negative and near zero relation
- Credit Score x Age: r = -0.011 - negative and near zero relation
- Balance x Estimated Salary: r = -0.013 - negative and near zero relation
- Balance x Credit Score: r = 0.017 - positive and near zero relation
- Estimated Salary x Credit Score: r = -0.055 - negative and near zero relation

All variables had the same behaviour, however, balance and credit score had the opposite behaviour in the churn group. While in the general analysis, the balance increases when the estimated salary increases (with a weak relation), in the churn group the balance decreases when the estimated salary increases. Nonetheless, a scatter plot was generated to demonstrate that there is no relationship between these two variables, as indicated by the absence of any discernible pattern in the graph.

## 9. Communication and Action

<img width="832" alt="Screen Shot 2024-10-14 at 8 26 59 PM" src="https://github.com/user-attachments/assets/5fd34860-dc70-46b6-9dcb-5eae9459fbe0">

## 10. SWOT Analysis

<img width="879" alt="Screen Shot 2024-10-14 at 8 28 30 PM" src="https://github.com/user-attachments/assets/46c3c0d6-1478-4afb-90a5-94abf1b09a22">


# References

Faritha Banu, J., Neelakandan, S., Geetha, B. T., Selvalakshmi, V., Umadevi, A., & Martinson, E. O. (2022). Artificial Intelligence Based Customer Churn Prediction Model for Business Markets. Computational intelligence and neuroscience, 2022, 1703696. https://doi.org/10.1155/2022/1703696 

Danao, M., Wats, R. What Is Churn Rate & How Do You Calculate It? (2024). Forbes
https://www.forbes.com/advisor/business/churn-rate/#:~:text=The%20churn%20rate%20refers%20to,customers%20are%20leaving%20your%20business 

Truta, F. (2018). High Churn Rate in Healthcare May Help Explain Sector’s Vulnerability to Phishing, Research Suggests. Bitdefender. https://www.bitdefender.com/en-us/blog/businessinsights/high-churn-rate-in-healthcare-may-help-explain-sectors-vulnerability-to-phishing-research-suggests/ 

Wilde. A. (2023). How to approach customer churn measurement in banking. UXPRESSIA. https://uxpressia.com/blog/how-to-approach-customer-churn-measurement-in-banking#Five_steps_to_stop_customers_from_leaving 

Michael, J. (2022). Bank Customer Churn Prediction Using Machine Learning. Analytics Vidhya. 
https://www.analyticsvidhya.com/blog/2022/09/bank-customer-churn-prediction-using-machine-learning/ 

Reichheld, F. (2021). Prescription for cutting costs. Bayn & Company.  https://media.bain.com/Images/BB_Prescription_cutting_costs.pdf 

Burns, J. (2024). How to reduce customer churn in banking. Unblu. 
https://www.unblu.com/en/blog/how-to-reduce-customer-churn-in-banking/ 

Picoult, J. (2023). The Limits Of Customer Love: A Cautionary Tale From First Republic Bank. Forbes. 
https://www.forbes.com/sites/jonpicoult/2023/05/03/the-limits-of-customer-love-a-cautionary-tale-from-first-republic-bank/ 

Toit, G., Glusac, N., Cuthell, K., Goossens, C., Gooyer, C. (2023). Customer Behavior and Loyalty in Banking: Global Edition 2023. Bain & Company. https://www.bain.com/insights/customer-behavior-and-loyalty-in-banking-global-edition-2023/ 
