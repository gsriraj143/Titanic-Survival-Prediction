# Titanic-Survival-Prediction 
📝 Project Overview : 
This project predicts whether a passenger on the Titanic survived the disaster using machine learning models. The dataset is part of the famous Kaggle Titanic Competition, and the goal is to build a robust model to predict survival based on passenger attributes such as gender, age, class, and more.
⚙️ Models Used
We evaluated several machine learning models and used an ensemble approach for the final prediction. Below are the models we tested:

Logistic Regression – Baseline model with 79.69% accuracy.
K-Nearest Neighbors (KNN) – Accuracy: 69.14%.
Support Vector Machine (SVM) – Accuracy: 69.60%.
Random Forest Classifier – Accuracy: 83.17%.
XGBoost Classifier – Accuracy: 83.50%.
The Voting Classifier (Random Forest + XGBoost) achieved the highest accuracy of 83.61% and was chosen for the final submission.

🛠️ Feature Engineering and Preprocessing
Missing Values Handling:
Age: Imputed with the median age grouped by Pclass and Sex.
Embarked: Filled with the mode value ("S").
Fare: Filled with the median fare.
Feature Engineering:
Created FamilySize by combining SibSp and Parch.
Created IsAlone feature if Family Size is 0 
Replaced less frequent values of Parch and SibSp with a single value
Cabin: Dropped due to more than 66% missing values.



