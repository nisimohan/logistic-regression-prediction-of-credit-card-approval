# Logistic Regression - Prediction of credit card approval

## Table of Contents
- [Problem Statement](#problemstatement)
- [Solution](#solution)
  - [Exploratory Data Analysis](#eda)
  - [Modeling](#modeling)
    - [Model1](#model1)
    - [Model2](#model2)
- [Conclusion](#conclusion)
- [Appendix](#appendix)

# Problem Statement

**Logistic Regression analysis and prediction of credit card approvals**

Companies have to go through a series of processes to approve a credit card for a person. This process is tedious and mundane. Every time an application is submitted bank has to analyze certain factors that play a vital role in the approval of the credit card, such as the income of the applicant, credit score, employment status, etc. This can be automated using Logistic regression analysis which can be used to understand the factors which have the most effect on the decision-making process of credit card approval. In order to achieve this, a logistic regression model can be trained to predict the probability of credit card approval based on the features from the data set. afterward, the trained logistic regression model can be analyzed to get insights into different features that have the highest impact on the approval rate.

# Solution

## Exploratory Data Analysis

We start off by understanding the type of data in the data frame. We can see from the below summary that there are 15 variables associated with credit card approval or denial. The outcome values of the last column approved are the following symbols, "+" means approved, and "-" means denied. These symbols are not meaningful, so we will be transforming them into 1's and 0's for the regression analysis.

There are five continuous variables in the dataset. We will check the relationship between these variables and credit card approval before jumping to regression analysis. A box plot is used here to understand the correlation between **Age_, Income, Debt, CreditScore, Years_Employed, and the approval rate**. The below box plots of these continuous variables show that the means of the features of the approved applications are further distributed from the mean of the denied.

![Box Plot: 1](screenshots/boxplot1.png)

