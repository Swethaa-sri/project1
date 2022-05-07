# project1

Problem Statement:
Financial threats are displaying a trend about the credit risk of commercial banks as the
incredible improvement in the financial industry has arisen. In this way, one of the
The biggest threats faced by commercial banks is the risk prediction of credit clients.
The goal is to predict the probability of credit default based on credit card owner's
characteristics and payment history.

EDA INSIGHTS:
Attributes: 25 and Row : 30,000
22% - default       78% - non – default
Defaults have a higher proportion of Lower LIMIT_BAL values
Non-Defaults have a higher proportion of Females (Sex=2)
Non-Defaults have a higher proportion of More Educated (EDUCATION=1 or 2)
Non-Defaults have a higher proportion of Singles (MARRIAGE=2)
Non-Defaults have a higher proportion of people 30-40years
Non-Defaults have a MUCH higher proportion of zero or negative PAY_X variables (this     means that being current or ahead of payments is associated with not defaulting in the following month).
The strongest predictors of default are the PAY_X (ie the repayment status in previous months), the LIMIT_BAL & the PAY_AMTX (amount paid in previous months).

Best Model:
Out of all classification model XGBOOST classifier perfomed best with roc_auc score of 78.04% and accuracy of 81.92%
Oversampling of dataset was done using smote and using the XGBOOST classifier accuracy 87% and roc_auc 93% for test set found.

Conclusion:
Conclusion: Using a XGBOOST classifier, we can predict with ~87% accuracy, whether a customer is likely to default next month.

The strongest predictors of default are the PAY_X (ie the repayment status in previous months), the LIMIT_BAL & the PAY_AMTX (amount paid in previous months).

Demographics: we see that being Female, More educated, Single and between 30-40years old means a customer is more likely to make payments on time.
