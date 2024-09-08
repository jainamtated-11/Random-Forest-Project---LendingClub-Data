# Random Forest Project - LendingClub Data

## Project Overview

This project explores publicly available data from **LendingClub.com**, which connects borrowers with investors. The primary objective is to create a machine learning model, specifically a **Random Forest classifier**, to predict whether borrowers will pay back their loans in full.

We focus on data from **2007-2010**, before LendingClub went public. The goal is to classify loan outcomes using various borrower features, providing investors with insight into potential risk.

## Dataset Information

The dataset contains a range of features related to the borrower and the loan. Here are some key columns:

- **credit.policy**: 1 if the borrower meets the LendingClub underwriting criteria, 0 otherwise.
- **purpose**: The reason for taking out the loan (e.g., "credit_card", "debt_consolidation").
- **int.rate**: The interest rate assigned to the loan.
- **installment**: Monthly payment amount for the loan.
- **log.annual.inc**: The natural log of the borrower's annual income.
- **dti**: The debt-to-income ratio of the borrower.
- **fico**: The borrower’s FICO credit score.
- **days.with.cr.line**: Number of days the borrower has had a credit line.
- **revol.bal**: The borrower’s revolving balance.
- **revol.util**: Revolving line utilization rate.
- **inq.last.6mths**: Number of creditor inquiries in the last 6 months.
- **delinq.2yrs**: Number of delinquent payments in the last 2 years.
- **pub.rec**: Number of public derogatory records (e.g., bankruptcies).

## Project Objectives

The primary goal of this project is to:
1. **Classify**: Determine whether a borrower will repay the loan in full.
2. **Predict**: Build a predictive model using the random forest algorithm.

## Steps in the Project

1. **Data Preprocessing**: Handle missing values, categorical encoding, and feature scaling.
2. **Exploratory Data Analysis (EDA)**: Analyze key features such as FICO scores, interest rates, and borrower income to identify trends.
3. **Model Building**: Train a **Random Forest classifier** using features such as credit policy, interest rates, and FICO scores.
4. **Model Evaluation**: Evaluate the model’s performance using metrics such as accuracy, precision, and recall.

## Exploratory Data Analysis (EDA)

### Key Insights:
- **FICO Score**: Borrowers with higher FICO scores tend to have lower interest rates.
- **Loan Purpose**: The majority of loans are for debt consolidation and credit card purposes.
- **Income**: Borrowers with higher annual income generally have lower debt-to-income ratios.
- **Interest Rates**: Riskier borrowers (as indicated by LendingClub's credit policy) are charged higher interest rates.

### Visualizations:
- **Distribution of FICO scores**: Plots showing the distribution of FICO scores across the dataset.
- **Interest Rates vs. Credit Policy**: Box plots comparing interest rates for those who meet LendingClub's credit policy vs. those who do not.

## Model Building

We utilized the **Random Forest Classifier** to predict loan repayment. Key steps:
1. **Train-Test Split**: Dividing the dataset into training and testing sets.
2. **Model Training**: Training the random forest model on the training set using features such as FICO score, credit policy, and loan purpose.
3. **Hyperparameter Tuning**: Optimizing parameters such as the number of trees and maximum depth using cross-validation.
4. **Model Evaluation**: Evaluating the model's predictive power on the test set.

## Results

- **Accuracy**: The Random Forest model achieved an accuracy of approximately `X%`.
- **Precision**: Precision was calculated at `Y%`, showing the proportion of correct positive predictions.
- **Recall**: Recall was measured at `Z%`, representing the model's ability to detect all positive instances.
- **Confusion Matrix**: A breakdown of true positives, false positives, true negatives, and false negatives.

## Conclusion

This project demonstrates the potential of machine learning in predicting loan repayment outcomes, giving investors a tool to assess borrower risk. The **Random Forest** model proved effective in classifying loan status, with promising accuracy and precision.

## Future Enhancements

1. **Feature Engineering**: Incorporating more features, such as economic indicators or additional borrower data.
2. **Model Optimization**: Experimenting with other algorithms, like Gradient Boosting or XGBoost.
3. **Time-Series Analysis**: Adding time as a feature to see how borrowing behavior changes over time.

