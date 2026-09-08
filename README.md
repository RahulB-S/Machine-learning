# 🚢 Titanic Survival Prediction

A machine learning project that predicts whether a passenger survived the Titanic disaster using **Python, Pandas, and Logistic Regression**.

## 📌 Project Overview

The goal of this project is to build a machine learning model that predicts passenger survival based on information such as:

- Passenger class
- Sex
- Age
- Number of siblings/spouses
- Number of parents/children
- Fare
- Port of embarkation

This project follows a complete beginner-friendly machine learning workflow:

**Data → Cleaning → Feature Engineering → Train/Test Split → Model Training → Prediction → Evaluation → Kaggle Submission**

## 🛠️ Technologies Used

- Python
- Pandas
- Scikit-learn
- Jupyter Notebook
- Kaggle
- GitHub

## 🧹 Data Preprocessing

The dataset was cleaned and prepared before training the model.

### Missing Values

- Missing `Age` values were replaced with the median age.
- Missing `Embarked` values were replaced with `"S"`.
- `Cabin` was removed because most of its values were missing.

### Encoding

The `Sex` column was converted into numerical values:

- Male → `1`
- Female → `0`

The `Embarked` column was converted using one-hot encoding.

### Removed Features

The following columns were removed for the initial model:

- `PassengerId`
- `Name`
- `Ticket`
- `Cabin`

## 🤖 Machine Learning Model

The project uses **Logistic Regression** from Scikit-learn.

The dataset was divided into:

- **80% training data**
- **20% validation data**

The model was then trained using the training data and evaluated on the validation data.

## 📊 Results

### Local Validation Accuracy

**81.0%**

### Kaggle Score

**76.7%**

The difference between the local validation accuracy and the Kaggle score shows why testing a model on unseen data is important.

## 🏆 Kaggle Submission

The trained model was used to generate predictions for Kaggle's test dataset.

The resulting `submission.csv` file was submitted to the Titanic competition and achieved a score of **0.767**.

## 📁 Project Structure

```text
titanic-survival-prediction/
│
├── proj1.ipynb
├── submission.csv
└── README.md