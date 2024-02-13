# Churn-Rate-Analysis

## Overview:
Churn Rate - Churn Rate is the rate at which customers stop doing business with a company over a given period of time. Churn may also apply to the number of subscribers who cancel or don't renew a subscription.
In this project, we are using a CSV file called "bank customer churn prediction.csv" to analyse the customer churn rate.

We have used Power Bi to visualise data.

## Steps:
  - Data Cleaning / Data Preparation
  - Data Modeling
  - Calculation and Analysis
  - Conclusion

## Data Cleaning / Preparation:
  -  The column 'Estimated Salary' is removed as it has no correlation with the churn rate.
  -  The data types of certain columns are changed.
  -  Spellings are checked and certain values are replaced.
  -  Table Columns such as Age, Account Balance and Credit Score have alot of distinct values which make it difficult to analyse. To avoid this, we group them by creating conditional columns.
  -  For better understanding of certain custom columns are created.

## Data Modeling:
  - It is always preferable to build distinct tables for each group and include a column that may be used to organize the numbers in a specific order based on age, balance, and credit score.
  - Done by using the 'Reference' method.
  - Create an index column based on certain conditions, hence we use conditional columns. 
  - We can see Customer data which is our Fact table and other reference tables such as Account balance groups, Credit Score group and Age group.
  - All of these columns have 'one to many' relationship with the customers data table.
    ![churn rate model](https://github.com/itsajayy/Web_Scraping-and-EDA/assets/135236892/3dfc424d-2bf6-4a42-8736-81019ce5487e)


## Calulations and Analysis:
  - Create new measures such as customer count and churn rate.
  - Churn Rate = (Customers left / Total Customer) * 100
  - Churn Rate of a particular company depends on the field of the company as well as the idealogy of the companies. I have taken the churn rate as 20% which is considered a bit high.
  - Donut visualisations are created using customer based on gender, product, activity status, country, credit card status.
  - Line and Clustered Column Charts are used to find the churn rate by different age groups.
  - Below is the dashboard:
    ![churn rate dashboard](https://github.com/itsajayy/Web_Scraping-and-EDA/assets/135236892/e61f5369-a10a-43c6-9f25-0c4135611166)


## Conclusion
  ### Inference
  - Churn Rate of this bank is 20.4%
  - Churn Rate os very high for customers who are in the age Group of 51-60 and for customers who have their credit score less than 400.
  - Customers with more than 200k in their account also then to have high churn rate.
  - Product 1 is most sold with more than 50% of the total product sales but it also has the highest churn rate of 27.7%
  - Product 2 has a churn rate of 7.6% but for customers from 1k - 10k account balance they have 100% churn rate.
  - Total Inactive Customers have 26.9% churn rate
  ### Recommendtaion
  - Implement targeted retention strategies specifically for customers in the age group of 51-60, as they exhibit a high churn rate.
  - Focus on improving services or providing incentives for customers with credit scores less than 400 to retain them.
  - Develop personalized services or benefits for customers with account balances exceeding 200k to enhance their loyalty and reduce churn.
  - Investigate the reasons behind the high churn rate for Product 1 despite its popularity. Consider optimizing the product or introducing additional features to increase customer.
  - Implement strategies to engage and re-activate inactive customers, as they have a significant churn rate. Provide targeted promotions or services to encourage their continued use of the bank's products.
  - Enhance communication strategies to educate customers about the benefits and features of the products, especially for those with lower credit scores or in the 51-60 age group.
  - Implement a system for continuous monitoring of churn rates and customer satisfaction. Regularly review and adjust strategies based on changing trends and customer feedback.
