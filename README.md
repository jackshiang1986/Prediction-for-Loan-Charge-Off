# Prediction for Loan Charge-Off

Project Description

For this project, a subset of LendingClud dataset from Kaggle will be used.

LendingClub is a US peer-to-peer lending company, headquartered in San Francisco, California. It was the first peer-to-peer lender to register its offerings as securities with the Securities and Exchange Commission (SEC), and to offer loan trading on a secondary market. LendingClub is the world's largest peer-to-peer lending platform.

Our Goal

Given historical data on loans given out with information on whether or not the borrower defaulted (charge-off), we will build machine learning models that can predict whether or nor a borrower will pay back their loan. This way in the future when we get a new potential customer we can assess whether or not they are likely to pay back the loan. The "loan_status" column, which contains our label, will later be converted into the target variable 'charge_off' for subsequent machine learning stage.

For this project, we will build several machine learning models using different algorithms, such as:

	i. Logistic Regression (linear)
	ii. AdaBoost Classifier (ensemble-boosting)
	iii. Gradient Boosting Classifier (ensemble-boosting)
	iv. Extreme Gradient Boosting (XGBoost) Classifier (ensemble-boosting)
	v. Random Forest (ensemble-bagging)
	vi. Neural Network (optimization-based)
For performance evaluation of models above, we will compare their area under curve (AUC) of receiver operating characteristic (ROC) curves, to see if any significant performance differences among different models. At the end of this notebook, a conclusion for this project will be presented.
