# Prediction for Loan Charge-Off

## Project Overview
For this project, a subset of LendingClud dataset ("lending_club_loan_two.csv") from Kaggle is used. This dataset contains the information of loans issued by LendingClub, and the records of the loan status at the end of the terms (“Fully Paid” or “Charged Off”). In this project, several machine learning models are built, which can be used to predict whether a borrower will pay back his or her loan. This way in the future when there are new potential customers, they can be assessed using the models for whether they are likely to pay back their loans.

For performance evaluation of different machine learning models, their area under curve (AUC) of receiver operating characteristic (ROC) curves are compared, to see if any significant performance differences among different models. At the end of this notebook, a conclusion for this project is presented.

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
At the beginning of the project, the dataset is first imported into the notebook (Prediction for Loan Charge Off.ipynb) and its structure and data types shall be checked. The dataset for this project has 396,030 rows and 27 columns.

The next thing to check is whether there are any missing values in the dataset. For the dataset of this project, there are some missing values. Several techniques can be used to deal with these missing values, such as dropping those rows with missing values (not recommended if the number of rows is too many), or imputing values into those missing fields based on other fields from the same dataset. For this project these 2 methods are used when dealing with the missing values.

After the missing values of the dataset are handled, the next step is to perform the exploratory data analysis (EDA). The distribution of each variable and how each independent variable relates to the dependent variable are checked. At the end of the EDA, several key observations can be drawn. In addition to the distributions of variables and their relationships with the dependent variable, any outliers in the dataset can also be found from the EDA. In this project, some thresholds are set for removing outliers.

For handling categorical variables, pandas get_dummied() method is used for creating dummy variables, whereas for numerical variables MinMaxScaler from sklearn is used for normalization.

For the machine learning stage, 70% of the dataset is used for training and 30% of the dataset is used for testing. For this project, several machine learning models are built using different algorithms. For performance evaluation of different models, their area under curve (AUC) of receiver operating characteristic (ROC) curves are compared. It is found that the performances of different models are quite similar, with the neural network and XGBoost classifier models are among the best. It is worth mentioning that during the machine learning stage, the Gradient Boosting Classifier spent significantly more time for training than XGBoost Classifier did, and obtained very similar performance. This once again shows that XGBoost Classifier is truely a very powerful and fast algorithm. Finally, at the end of the project notebook, the conclusion for this project is presented.

The following documents are provided in this repository:
  1. Prediction for Loan Charge Off.ipynb: Notebook for Python codes of the project
  2. lending_club_loan_project_data.rar: Dataset for the project
