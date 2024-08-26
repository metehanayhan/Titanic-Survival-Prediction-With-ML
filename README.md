# Titanic Survival Prediction

This repository contains a machine learning project aimed at predicting the survival of passengers aboard the Titanic. The project is developed as part of a Kaggle competition and utilizes various classification algorithms to achieve accurate predictions.

## Introduction
The sinking of the Titanic is one of the most infamous shipwrecks in history. On April 15, 1912, during her maiden voyage, the Titanic sank after colliding with an iceberg, killing 1502 out of 2224 passengers and crew. This project aims to predict whether a passenger would survive the disaster based on various features like age, gender, and class.

## Dataset
The dataset used in this project is provided by Kaggle and can be found [here](https://www.kaggle.com/competitions/titanic/data). It includes information about the passengers, such as:
- `PassengerId`: Unique ID for each passenger
- `Survived`: Survival (0 = No; 1 = Yes)
- `Pclass`: Ticket class (1 = 1st; 2 = 2nd; 3 = 3rd)
- `Name`: Name of the passenger
- `Sex`: Gender
- `Age`: Age in years
- `SibSp`: Number of siblings/spouses aboard the Titanic
- `Parch`: Number of parents/children aboard the Titanic
- `Ticket`: Ticket number
- `Fare`: Passenger fare
- `Cabin`: Cabin number
- `Embarked`: Port of Embarkation (C = Cherbourg; Q = Queenstown; S = Southampton)

## Features
The following features were engineered and selected for the model:
- **Age**: Filled missing values using median.
- **Fare**: Used log transformation to normalize the distribution.
- **Embarked**: Imputed missing values and converted to dummy variables.
- **Pclass**: Treated as a categorical variable.
- **FamilySize**: Created by combining SibSp and Parch.

## Modeling
The following machine learning algorithms were used in this project:
- Logistic Regression
- Decision Trees
- Random Forest
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)

### Model Evaluation
Models were evaluated using accuracy, precision, recall, and F1-score. Cross-validation was employed to ensure robustness.

## Results
The Random Forest model achieved the highest accuracy on the test set. Detailed results and performance metrics for each model are provided in the notebook.

![Kaggle-Score](https://github.com/user-attachments/assets/402765f5-b07a-4f08-a9ba-3b57bf0045b9)
