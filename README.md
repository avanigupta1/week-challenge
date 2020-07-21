# Week-Long Data Science Challenge

Binary classification system reviewing lead conversion behavior. 

## Contents

### [Exploratory Data Analysis](https://github.com/avanigupta1/week-challenge/blob/master/EDA.ipynb)
- Reviewing variable relationships to the target and to each other. 
- Reviewing and combining lower levels in categorical data.
- Reviewing and transforming numerical variables.

### [Missing Data Analysis](https://github.com/avanigupta1/week-challenge/blob/master/Missing%20Data%20Review.ipynb)
- Exploring methods of missing data
- Imputing most frequent inputs for variables with either low missing-ness or those that are highly skewed
- Using KNN imputation methods for other missing variables
- Using SMOTE oversampling methods to create a dataset that has class balance for further modeling research

### [Baseline Models](https://github.com/avanigupta1/week-challenge/blob/master/Baseline%20Models.ipynb)
- Run various models on cleaned & imputed dataset; review performance scores.
- Models:
  - Logistic Regression
  - Decision Tree Classifier
  - Linear Discriminant Analysis
  - Quadratic Discriminant Analysis
  - Random Forest Classifier
  - Naive Bayes
  - XGBoost
  - Basic Neural Network
  - CatBoost

### Tuning
### [Neural Network Tuning](https://github.com/avanigupta1/week-challenge/blob/master/Neural%20Network%20Tuning.ipynb)
Using imputed and one hot encoded data, tested out basic neural network modeling in addition to layer and experimentation. Incorproated embedding layers for text data and created combined model with specific segments for text, categorical, and numerical data. 

Result: Minimal to negative improvement when testing out various iterations. 

### [XGBoost](https://github.com/avanigupta1/week-challenge/blob/master/XGBoost%20Tuning.ipynb)
Using imputed and one hot encoded data, reviewed feature importances.

Result: When removing unimportant features, performance dropped.

### CatBoost
#### [Missing Data](https://github.com/avanigupta1/week-challenge/blob/master/CatBoost%20-%20Missing%20Data.ipynb)
Performed CatBoost training on dataset with missing values. Though CatBoost is known to work well with missing data, feature importances on first iteration showed a highly skewed variable to be most important, which empirically does not make sense. When removing said variable, performance dropped.
#### [SMOTE Data](https://github.com/avanigupta1/week-challenge/blob/master/CatBoost%20-%20SMOTE%20Data.ipynb)
Tested SMOTE oversampled dataset to see veracity of data. Though performance was incredibly high, when testing on validation set un-touched by SMOTE methods, performance deeply declined lower than that of baseline models.
#### [Tuning on Imputed Data Set](https://github.com/avanigupta1/week-challenge/blob/master/CatBoost%20-%20Tuning.ipynb)
Final dataset and modeling method chosen. Tuned by using GridSearch on variety of parameters. Explored various threshold points for binary classification. 
##### [Tuned Model Interpreptation](https://github.com/avanigupta1/week-challenge/blob/master/Model%20Interpretation.ipynb)
Feature importance and tree diagram visualized from tuned model. 

