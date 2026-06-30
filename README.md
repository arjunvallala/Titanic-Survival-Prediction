# Titanic Survival Prediction

## Project Overview

This project analyzes the Titanic dataset from Kaggle and predicts whether a passenger survived based on passenger information. The project covers the complete machine learning workflow, including data preprocessing, exploratory data analysis (EDA), feature engineering, model training, and generating predictions for the Kaggle competition.

Dataset: https://www.kaggle.com/competitions/titanic

---

## Dataset

The dataset contains information about Titanic passengers such as:

- Passenger Class (Pclass)
- Name
- Sex
- Age
- Siblings/Spouses Aboard (SibSp)
- Parents/Children Aboard (Parch)
- Fare
- Embarked
- Survival Status (Training data only)

---

## Data Preprocessing

The following preprocessing steps were performed:

- Filled missing values in the **Age** column using the mean age.
- Filled missing values in the **Embarked** column.
- Dropped the **Cabin** column because it contained a large number of missing values.
- Dropped the **Ticket** column.
- Applied One-Hot Encoding to categorical columns:
  - Sex
  - Embarked

---

## Exploratory Data Analysis (EDA)

Several visualizations and analyses were performed to understand the dataset.

### Key Observations

- Female passengers had a higher survival rate than male passengers.
- Passengers who boarded from Southampton (S) had a higher death rate.
- Older passengers (Age 60–100) showed the highest death ratio.
- Third-class passengers had the highest death ratio, followed by second class, while first-class passengers had the highest survival rate.
- Passengers traveling with one sibling or spouse had a better survival rate than those traveling alone.
- Passengers traveling with one, two, or three parents/children generally showed better survival rates.
- First-class passengers were generally older than passengers in second and third class.
- Female passengers tended to travel with more family members compared to male passengers.
- Fare was strongly related to passenger class, with first-class passengers paying significantly higher fares.

Various plots such as bar charts, histograms, box plots, scatter plots, pie charts, and violin plots were used during the analysis.

---

## Features Used

The following features were used for prediction:

- Sex
- Embarked
- Age
- Pclass
- SibSp
- Parch
- Fare

---

## Files

```
Titanic-Survival-Prediction/
│
├── Titanic_Survival_Prediction.ipynb
├── train.csv
├── test.csv
├── submission.csv
├── requirements.txt
└── README.md
```

---

## Requirements

Install the required libraries using:

```bash
pip install -r requirements.txt
```

---

## Libraries Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

---

## Kaggle Submission

After preprocessing the test dataset using the same steps as the training data, predictions were generated and saved as **submission.csv**, which can be uploaded directly to the Kaggle Titanic competition.

---

## What I Learned

Through this project, I learned how to:

- Load and explore datasets using Pandas.
- Handle missing values.
- Perform exploratory data analysis (EDA).
- Visualize data using Matplotlib and Seaborn.
- Encode categorical features.
- Split data into training and testing sets.
- Train a machine learning model.
- Generate predictions on unseen data.
- Create a submission file for a Kaggle competition.
