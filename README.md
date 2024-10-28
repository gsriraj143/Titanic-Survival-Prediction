# Titanic-Survival-Prediction 


## 📝 Project Overview : 
This project predicts whether a passenger on the Titanic survived the disaster using machine learning models. The dataset is part of the famous Kaggle Titanic Competition, and the goal is to build a robust model to predict survival based on passenger attributes such as gender, age, class, and more.

## 📂Importing Libraries

In this project, I **import essential libraries** that play pivotal roles in enhancing data manipulation and visualization capabilities:

- **pandas**: A versatile library for data manipulation and analysis, enabling me to handle tabular data structures effectively.
- **numpy**: A fundamental library for numerical operations and computations, empowering me with efficient mathematical operations on arrays.
- **seaborn**: A powerful data visualization library based on matplotlib, simplifying the creation of informative statistical graphics.
- **matplotlib.pyplot**: A widely used library for creating plots and charts, crucial for visualizing my data and analysis results effectively.

## ⚙️ EDA (Exploratory Data Analysis)
In **Exploratory Data Analysis (EDA)**, I dive deep into understanding the dataset. Using various visualization techniques, I : 
- Visualize the distributions of key numerical features such as age, number of siblings/spouses (SibSp), number of parents/children (Parch), and fare to identify trends and detect outliers.
- Analyze relationships between variables to uncover potential correlations that might influence survival predictions.
                                       
Insights from Visualizations:
- Gender: Females had a higher survival rate than males.
- Passenger Class: Passengers from 1st class were more likely to survive compared to those in 3rd class.
- Embarked Port: Passengers from Cherbourg (C) had higher survival rates.




                                                                                                                                                            
## 🛠️ Feature Engineering and Preprocessing   

Missing Values Handling:
- Age: Imputed with the median age grouped by Pclass and Sex.                                                                                                
- Embarked: Filled with the mode value ("S").                                                                                                                
- Fare: Filled with the median fare.

Feature Engineering:
- Created FamilySize by combining SibSp and Parch.                                                                                                           
- Created IsAlone feature if Family Size is 0                                                                                                                
- Replaced less frequent values of Parch and SibSp with a single value                                                                                      
- Cabin: Dropped due to more than 66% missing values.  

## 🚀 Models Used 


We evaluated several machine learning models and used an ensemble approach for the final prediction. Below are the models we tested:

- Logistic Regression – Baseline model with 79.69% accuracy.                                                                          
- K-Nearest Neighbors (KNN) – Accuracy: 69.14%.                                                                                                              
- Support Vector Machine (SVM) – Accuracy: 69.60%.                                                                                                           
- Random Forest Classifier – Accuracy: 83.17%.                                                                                                               
- XGBoost Classifier – Accuracy: 83.50%.
- The **Voting Classifier (Random Fores XGBoost)** achieved the highest accuracy of 83.61% and was chosen for the final submission.

## 📁 Submission
We generated predictions with the final Voting Classifier and saved them in the required Kaggle submission format - **Predictions.csv**

## Conclusion

At a predictive accuracy of **83.7%**, my model demonstrates its potential to forecast Titanic passenger survival effectively. This project not only illustrates the practical application of machine learning techniques on historical data but also provides insights into the influential factors behind survival rates during the Titanic disaster.




