# Titanic Survival Prediction (Kaggle)

##  Project Overview
This project aims to predict whether a passenger survived the Titanic disaster using machine learning techniques.  
The dataset is taken from the famous **Kaggle Titanic: Machine Learning from Disaster** competition.

This project demonstrates a complete **end-to-end machine learning workflow**, including data cleaning, feature encoding, model training, evaluation, and Kaggle submission.

---

##  Dataset
- Source: Kaggle Titanic Competition
- Files used:
  - `train.csv` – contains features and target variable (`Survived`)
  - `test.csv` – contains features only (no target)

 Note: Dataset files are **not included** in this repository due to Kaggle’s data usage policy.

---

##  Tools & Technologies
- Python
- Pandas
- NumPy
- Scikit-learn
- Google Colab / Jupyter Notebook

---

##  Features Used
- Pclass
- Sex
- Age
- SibSp
- Parch
- Fare
- Embarked (one-hot encoded)

---

##  Data Preprocessing
- Handled missing values:
  - Age → filled with median
  - Embarked → filled with most frequent value
  - Fare (test data) → filled with median
- Encoded categorical variables:
  - Sex → label encoding
  - Embarked → one-hot encoding
- Ensured train and test datasets have aligned feature columns

---

##  Model Used
- **Logistic Regression**
- Train-validation split used for local evaluation
- Final model trained on full training dataset

---

##  Model Performance
- Validation Accuracy: ~81%
- Kaggle Public Score: **0.76**

---

##  Kaggle Submission
- Submission file contains only:
  - `PassengerId`
  - `Survived`

Kaggle Competition Link:  
https://www.kaggle.com/competitions/titanic

---

##  Learning Outcomes
- Understanding of ML pipeline
- Handling missing data
- Feature encoding techniques
- Difference between validation data and Kaggle test data
- Real-world ML competition workflow

---

##  Future Improvements
- Feature engineering (FamilySize, IsAlone, Title extraction)
- Try advanced models like Random Forest or Gradient Boosting
- Hyperparameter tuning
- Cross-validation
