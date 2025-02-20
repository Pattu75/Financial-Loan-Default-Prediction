Financial Loan Default Prediction

1. Project Overview:

This project focuses on predicting loan defaults using machine learning techniques. Financial institutions aim to minimize loan payment defaults 
by identifying high-risk borrowers early. The goal is to build a predictive model that can accurately determine the likelihood of a borrower defaulting 
on their loan payments.

2. Dataset:

The dataset consists of two main files:

train.csv: Contains 255,347 loan records with 18 features, including the target variable Default (1 if the borrower defaulted, 0 otherwise).

test.csv: Contains 109,435 loan records with the same features as train.csv, but without the Default column. The task is to predict the probability 
of default for these loans.

3. Exploratory Data Analysis (EDA):

Data Cleaning: The dataset contains no missing values or duplicates.

Target Variable: Approximately 11.61% of loans in the training set defaulted.

Feature Analysis: Younger borrowers and those with lower credit scores are more likely to default. Employment type and marital status also influence 
default rates.

4. Model Development:

Baseline Model: A DummyClassifier was used to establish a baseline performance. Different strategies (stratified, prior, uniform) were tested, with the 
prior strategy achieving the highest accuracy (88.39%).

Logistic Regression: Achieved an AUC score of 0.7281, indicating moderate predictive power.

Random Forest: A GridSearchCV was used to optimize hyperparameters, resulting in an improved AUC score.

5. Model Evaluation:

Cross-Validation: The baseline model achieved a mean cross-validation accuracy of 88.39%.

AUC Score: The Random Forest model achieved a higher AUC score compared to Logistic Regression, indicating better performance in distinguishing 
between default and non-default loans.

6. Conclusion:

The project demonstrates the use of machine learning to predict loan defaults. While the baseline model provides a starting point, more sophisticated 
models like Random Forest show promise in improving prediction accuracy. Future work could involve exploring additional algorithms, feature engineering, 
and hyperparameter tuning to further enhance model performance.
- Experiment with additional machine learning algorithms (e.g., Gradient Boosting, XGBoost).
- Perform feature engineering to create new features that may improve model performance.
- Deploy the model in a production environment for real-time predictions.

This project provides a solid foundation for predicting loan defaults and can be extended to address more complex scenarios in financial risk management.

