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

So what is some codes na andito nga ba? so for example " data = pd.read_csv("../data/diabetes.csv")
" Binabasa nito yung CSV file ng dataset at data = table ng lahat ng patients. and also for example yung " scaler = StandardScaler()
X_train_scaled = scaler.fit_transform(X_train)
X_test_scaled = scaler.transform(X_test) " ito naman yung pag-scale ng features para pareho ang importance sa model ,tinuturo sa scaler yung mean at std ng training data, tapos ginagamit para i-scale at pag ginagamit lang yung scaler sa testing data.

and yung " joblib.dump(model, "../diabetes_model.pkl")
joblib.dump(scaler, "../scaler.pkl") " namn ay pag Sinisave natin yung model at scaler sa file Para next time hindi na kailangan i-train uli.


