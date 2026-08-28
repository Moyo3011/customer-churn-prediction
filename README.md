# Customer Churn Prediction Project

## Business Problem

This project looks at customer churn for a telco company that provides home phone and internet services in California. The company is losing customers, which can affect its revenue. So the aim of the project is to use customer data to understand why customers may leave(churn) and see if machine learning can help predict which customers are more likely to churn.

## Project Question

What factors are linked to customer churn, and can machine learning help identify customers who may be at risk of leaving?

## Machine Learning Objective

The aim of the models is to predict whether a customer is likely to churn or stay based on information about the customer, such as their contract, how long they have been with the company and how much they pay.

## Input Features

The project uses information about:
- Customer details: gender, senior citizen status, partner and dependents
- Account details: tenure, contract type and payment method
- Services: internet service, phone service, online security and technical support
- Charges: monthly charges and total charges

## Output Prediction

The models predict whether a customer is:
- Likely to churn (Yes)
- Likely to stay (No)

## Dataset

The project uses the Telco Customer Churn dataset, which contains information about 7,043 customers and 21 features. It includes information about customer details, accounts, services, charges and whether the customer churned.

## Tools Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Steps

The project included:

1. Understanding the data
2. Cleaning the data
3. Exploring the data
4. Preparing the data for machine learning
5. Building a Logistic Regression model
6. Building a Random Forest model
7. Comparing the models
8. Looking at the main findings and possible business actions

## Key Findings

Some of the main findings from the analysis were:

* Month to month customers had a much higher churn rate than customers on longer contracts. The churn rate was 42.71% for month to month customers, compared with 11.27% for one year contracts and 2.83% for two year contracts.
* Customers with shorter tenure appeared more likely to churn.
* TotalCharges, tenure and MonthlyCharges were the three most important features in the random forest model.
* Some services and payment methods also showed differences in churn behaviour.

## Model Results

Two models were tested:

### Logistic Regression
- Accuracy: 81.0%
- Precision: 66%
- Recall: 57%
- F1-Score: 61%
- ROC-AUC: 0.842

### Random Forest
- Accuracy: 78.5%
- Precision: 62%
- Recall: 50%
- F1-Score: 55%
- ROC-AUC: 0.825

Logistic regression performed better than random forest on this dataset. It also identified a higher percentage of customers who actually churned, with a churn recall of 57% compared with 50% for random forest.

## Recommendations

Based on the findings the company could:
- Look at ways to encourage month to month customers to move to longer contracts.
- Give newer customers more support during their first few months.
- Look into whether customers with higher monthly charges feel they are getting good value.
- Investigate the differences seen between different services and payment methods.
- Use the model to help identify customers who may be more likely to churn.

These findings show possible areas for the company to investigate, but they do not prove that these factors directly cause customers to churn.

## Limitations

The analysis shows patterns in the dataset but does not prove that a particular factor directly causes a customer to churn. The models were also tested on this particular dataset, so their results may be different when used with new customer data.

## Project File

- `customer_churn_analysis.ipynb` — Contains the data analysis, graphs, machine learning models and results.
