# Prediction for Loan Charge-Off

## Project Overview
For this project, a subset of LendingClud dataset ("lending_club_loan_two.csv") from Kaggle was used. This dataset contains the information of loans issued by LendingClub, and the records of the loan status at the end of the terms (“Fully Paid” or “Charged Off”). In this project, several machine learning models were built, which could be used to predict whether a borrower will pay back his or her loan. 

For performance evaluation of different machine learning models, their area under curve (AUC) of receiver operating characteristic (ROC) curves were compared, to see if any significant performance differences among different models. At the end of this notebook, a conclusion for this project was presented.

## Objectives of the Project
The following are the objectives of the project:
1.	Build and train machine learning models for the prediction of loan charge-off using different algorithms, such as:
    *	Logistic Regression (linear)
    *	AdaBoost Classifier (ensemble-boosting)
    *	Gradient Boosting Classifier (ensemble-boosting)
    *	Extreme Gradient Boosting (XGBoost) Classifier (ensemble-boosting)
    *	Random Forest (ensemble-bagging)
    *	Neural Network (optimization-based)
2.	Compare the performances of different machine learning models in terms of their AUC of ROC curves.

## Project Outline
At the beginning of the project, the dataset was first imported into the notebook (Prediction for Loan Charge Off.ipynb) and its structure and data types were checked. There were 396,030 rows and 27 columns for this dataset.

The next thing to check was whether any missing values in the dataset. For the dataset of this project, there were some missing values. Several techniques could be used to deal with these missing values, such as dropping those rows with missing values (not recommended if large number of rows), or imputing values into those missing fields based on other fields from the same dataset. For this project these 2 methods were used when dealing with the missing values.

After the missing values of the dataset were handled, the next step was to perform the exploratory data analysis (EDA). The distribution of each variable and how each independent variable related to the dependent variable were checked. At the end of the EDA, several key observations could be drawn. In addition to the distributions of variables and their relationships with the dependent variable, any outliers in the dataset could also be found from the EDA. In this project, some thresholds were set for removing outliers.

For handling categorical variables, pandas get_dummied() method was used for creating dummy variables, whereas for numerical variables MinMaxScaler from sklearn was used for normalization.

For the machine learning stage, 70% of the dataset was used for training and 30% of the dataset was used for testing. For this project, several machine learning models were built using different algorithms. For performance evaluation of different models, their area under curve (AUC) of receiver operating characteristic (ROC) curves were compared. It was found that the performances of different models were quite similar, with the neural network and XGBoost classifier models were among the best. Finally, at the end of the project notebook, the conclusion for this project was presented.

The following documents are provided in this repository:
  1. Prediction for Loan Charge Off.ipynb: Notebook for Python codes of the project
  2. lending_club_loan_project_data.rar: Dataset for the project
