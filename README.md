# Prediction for Loan Charge-Off

For this project, a subset of LendingClud dataset from Kaggle will be used.

LendingClub is a US peer-to-peer lending company, headquartered in San Francisco, California. It was the first peer-to-peer lender to register its offerings as securities with the Securities and Exchange Commission (SEC), and to offer loan trading on a secondary market. LendingClub is the world's largest peer-to-peer lending platform.

Given historical data on loans given out with information on whether or not the borrower defaulted (charge-off), we will build machine learning models that can predict whether or not a borrower will pay back his or her loan. This way in the future when we get new potential customers we can assess whether they are likely to pay back their loans. The "loan_status" column, which contains our label, will later be converted into the target variable 'charge_off' for subsequent machine learning stage.

For this project, we will build several machine learning models using different algorithms, such as:

* Logistic Regression (linear)
* AdaBoost Classifier (ensemble-boosting)
* Gradient Boosting Classifier (ensemble-boosting)
* Extreme Gradient Boosting (XGBoost) Classifier (ensemble-boosting)
* Random Forest (ensemble-bagging)
* Neural Network (optimization-based)

For performance evaluation of models above, we will compare their area under curve (AUC) of receiver operating characteristic (ROC) curves, to see if any significant performance differences among different models. At the end of this notebook, a conclusion for this project will be presented.

The following documents are provided in this repository:
  1. Prediction for Loan Charge Off.ipynb: Notebook for Python codes of the project
  2. lending_club_loan_project_data.rar: Dataset for the project
