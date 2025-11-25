# kaggle_titanic_competition_entry
**Titanic Survival Prediction – Machine Learning Project**
This project solves the classic Titanic Survival Prediction challenge on Kaggle.
The goal is to build machine learning models that predict whether a passenger survived the Titanic shipwreck using demographic and travel-related information.

**Project Overview**

The Kaggle Titanic dataset is a beginner-friendly classification problem involving:

Binary classification (0 = did not survive, 1 = survived)

Missing values (Age, Cabin, Embarked)

Categorical variables (Sex, Embarked, Pclass)

Feature engineering opportunities

Model comparison & evaluation

This project achieves a Kaggle leaderboard score of 0.77, improving from an initial 0.75.

**Objectives**
Explore and clean the dataset

Handle missing values

Encode categorical features

Perform feature engineering

Train and evaluate multiple ML models

Improve performance through model tuning

Generate submission files for Kaggle

**Dataset**

The dataset comes from Kaggle’s Titanic: Machine Learning from Disaster competition.

Files:

train.csv – training data with labels

test.csv – test data without labels

gender_submission.csv – sample submission

**Target variable:**

Survived (0 = No, 1 = Yes)

**Data Preprocessing**

Key steps performed:

✔ Handling Missing Values

Age → filled using median age

Embarked → mode

Cabin → filled as “Unknown” (optional grouping by cabin letter)

✔ Encoding Categorical Features

Sex → mapped to numeric (0 = male, 1 = female)

Embarked → one-hot encoded

✔ Feature Engineering

Extracted Title from names (Mr, Mrs, Miss, etc.)

**Models Used**
Logistic Regression

Baseline model

Kaggle Score: 0.75

Random Forest Classifier

Better handling of nonlinear patterns

Kaggle Score: 0.77

Gradient Boosting Classifier

Stronger boosting model

Kaggle Score: 0.77

Often performs well with fewer hyperparameters

Model Performance (Local Validation)
Model	Validation Accuracy
Logistic Regression	~0.80
RandomForestClassifier	~0.84
GradientBoostingClassifier	~0.85

Kaggle scores are lower because the leaderboard tests on unseen data.
