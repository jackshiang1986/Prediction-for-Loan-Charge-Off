# Prediction for Loan Charge-Off

## Project Overview
For this project, a subset of LendingClud dataset ("lending_club_loan_two.csv") from Kaggle will be used. This dataset contains the information of loans issued by LendingClub, and the records of the loan status at the end of the terms (“Fully Paid” or “Charged Off”). In this project, we will build machine learning models that can predict whether a borrower will pay back his or her loan. This way in the future when we get new potential customers, we can assess whether they are likely to pay back their loans.

## Project Outline
At the beginning of the project, we will first import the dataset into the notebook and check its structure and data types. The dataset for this project has 396,030 rows and 27 columns.

The next thing to check is whether there are any missing values in the dataset. For the dataset of this project, we do have missing values. Several techniques can be used to deal with these missing values, such as dropping those rows with missing values (not recommended if the number of rows is too large), or imputing values into those missing fields based on other fields from the same dataset. For this project these 2 methods are used when dealing with the missing values.

After the missing values of the dataset have been handled, the exploratory data analysis (EDA) for the dataset can be performed. For the distribution of each variable will be checked, and how each independent variable relates to the dependent variable. At the end of the EDA, several key observations from the EDA can be drawn. In addition to the distributions of variables and their relationships with the dependent variables, we can also find if there are any outliers in the dataset. In this project, some thresholds are set for removing outliers.

For handling categorical variables, we will use pandas get_dummied() method for creating dummy variables, whereas for numerical variables we will use MinMaxScaler from sklearn for normalization.

For the machine learning, we will use 70% of the dataset for training and 30% of the dataset for testing. For this project, we will build several machine learning models using different algorithms, such as:
*	Logistic Regression (linear)
*	AdaBoost Classifier (ensemble-boosting)
*	Gradient Boosting Classifier (ensemble-boosting)
*	Extreme Gradient Boosting (XGBoost) Classifier (ensemble-boosting)
*	Random Forest (ensemble-bagging)
*	Neural Network (optimization-based)

For performance evaluation of models above, we will compare their area under curve (AUC) of receiver operating characteristic (ROC) curves, to see if any significant performance differences among different models. At the end of the project notebook, a conclusion for this project will be presented.

The following documents are provided in this repository:
  1. Prediction for Loan Charge Off.ipynb: Notebook for Python codes of the project
  2. lending_club_loan_project_data.rar: Dataset for the project
