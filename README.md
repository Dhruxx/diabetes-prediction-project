# diabetes-prediction-project
The dataset used for this project is the Diabetes Dataset from Kaggle. It contains various medical and demographic features that influence diabetes diagnosis. The key features include:

Pregnancies: Number of times the patient has been pregnant.

Glucose: Plasma glucose concentration.

BloodPressure: Diastolic blood pressure (mm Hg).

SkinThickness: Triceps skin fold thickness (mm).

Insulin: 2-Hour serum insulin (mu U/ml).

BMI: Body mass index (weight in kg/(height in m)^2).

DiabetesPedigreeFunction: A function that represents the likelihood of diabetes based on family history.

Age: Age of the patient in years.

Outcome: Target variable (0 = No Diabetes, 1 = Diabetes).

Preprocessing Steps

To ensure optimal model performance, the following preprocessing steps were taken:

Data Cleaning:

Checked for missing values and inconsistencies.

No missing values were found, so no imputation was needed.

Exploratory Data Analysis (EDA):

Generated a correlation heatmap to analyze feature relationships.

Plotted distributions of key features.

Feature Scaling:

Used StandardScaler to normalize numerical features for better model performance.

Data Splitting:

The dataset was split into training and testing sets (80%-20% split).

Models Trained and Performance

We trained the following classification models to predict diabetes:

Model

Accuracy

Precision

Recall

F1-Score


Key Findings:

XGBoost performed the best in terms of overall accuracy and F1-score.

Random Forest also performed well with high precision and recall.

Logistic Regression was used as the baseline model and performed reasonably.

Decision Tree had higher variance but was interpretable.

Additional Evaluation

Confusion Matrix: Visualized the number of True Positives, False Positives, True Negatives, and False Negatives for each model.

ROC Curve: Plotted to compare model performance in terms of sensitivity and specificity.

Hyperparameter Tuning

GridSearchCV was applied to Random Forest to find the best combination of hyperparameters.

The best parameters improved accuracy and overall performance.

Conclusion

This project demonstrated the importance of feature engineering and model selection in diabetes prediction. Future work could explore additional feature selection techniques, deep learning models, or larger datasets for better generalization.
