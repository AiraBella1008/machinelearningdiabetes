This project uses a supervised machine learning algorithm (Logistic Regression)
to predict whether a patient has diabetes using the Kaggle Pima Indians dataset.

Source: Kaggle
Includes health metrics:
- Glucose
- BMI
- Age
- Insulin
- Blood pressure
- ...etc


So i Used used pandas to read and manipulate datasets (CSV files and ogisticRegression for the ML model to predict whether a patient has diabetes (Outcome=1) or not (Outcome=0).
and as you can see i put  StandardScaler standardizes numeric features so they have mean = 0 and std = 1. This helps the model converge faster and perform better
