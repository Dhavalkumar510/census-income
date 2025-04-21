# 📊 Census Income Classification Using Machine Learning

## 📌 Introduction
This project focuses on classifying individuals based on their income levels (<=50K or >50K) using the Census Income dataset. The complete pipeline involves data exploration, preprocessing, model training, and evaluation using Decision Tree and Random Forest classifiers.

## 🔍 Exploratory Data Analysis (EDA)
The analysis began with loading the dataset and performing initial exploratory steps:

Displayed the first few rows

Generated descriptive statistics

Visualized the distribution of key variables

Focused on understanding the capital-gain feature

## 📌 Key Parameters Considered:
Age – Relationship between age and income level

Education Level – Correlation between education and income

Occupation – Impact of job roles on earnings

Marital Status – Influence on income trends

Capital Gains/Losses – Investment-related factors

Hours per Week – Relationship to earning potential

Income Bracket – <=50K vs >50K

## 📈 Income Class Distribution:
Using a count plot, the income class distribution was visualized:

<=50K → 75.92%  &  >50K → 24.08%

## 🛠️ Data Preprocessing
Cleaned and encoded the income column into a binary format (income_code)

Selected relevant features for training

Split data into train and test sets

## 🌳 Decision Tree Classifier
Built a Decision Tree model

Used GridSearchCV for hyperparameter tuning

Evaluated using accuracy and ROC curve

Visualized the resulting tree to understand decisions

## 🌲 Random Forest Classifier
Built a Random Forest model

Applied RandomizedSearchCV for hyperparameter optimization

Evaluated using a confusion matrix and classification report

Provided robust performance with better generalization

## ⚖️ Addressing Class Imbalance with SMOTE
To improve model robustness, SMOTE was used:

Oversampled the minority class (>50K)

Improved balance and predictive performance

## 📌 Feature Selection with RFE
Employed Recursive Feature Elimination (RFE) to select most important features

Performed for both Decision Tree and Random Forest models

Highlighted which variables contributed most to model accuracy

## 📊 Accuracy Comparison
A bar plot comparison was created to visualize:

Decision Tree Accuracy

Random Forest Accuracy

Random Forest outperformed Decision Tree with:

Better accuracy

Improved handling of high-dimensional data

## ✅ Key Insights
Decision Tree: Useful for interpretability and initial model building

Random Forest: Excellent for predictive accuracy and feature importance

Best Accuracy: 0.82 (after handling class imbalance with SMOTE)

## 🧠 Conclusion
The project successfully demonstrates the use of machine learning for income prediction:

Started with solid EDA

Applied robust classification techniques

Addressed imbalance with SMOTE

Used RFE for intelligent feature selection

Compared and evaluated models thoroughly

The final model provides a well-rounded foundation for understanding socio-economic factors influencing annual income and can be further refined for real-world applications.

## 🚀 Future Improvements
Apply ensemble methods like XGBoost or LightGBM

Incorporate cross-validation

Automate hyperparameter search using Optuna

Build a web app for interactive predictions

