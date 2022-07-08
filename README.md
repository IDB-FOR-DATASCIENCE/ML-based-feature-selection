# Feature Selection - Classification
_**Code Pipeline for using multiple feature selection methods for classification purpose**_

---

---


## Contents

1. [Purpose](#Purpose)
2. [Steps](#Steps)
3. [Data](#Data)
4. [Instructions](#Instructions)



## Purpose:

_This notebook is a one stop shop for ML based feature selection for classification purpose. Once the master data is prepared, we can use this notebook to try out 8 feature selection techniques and combine their results_



## Steps:

### Step 1: Load Package and Custom Functions

1. Install/Import necesarry packages
2. Load custom functions
3. Input user defined metrics


### Step 2: Data Preparation:

1. Import dataset
2. Profiling and EDA
3. Drop unwanted fields and convert column types
4. Null Treatment
5. Treating categorical features (one hot encoding, WOE encoding)
6. Train/Test/OOT Split


### Step 3: Feature Selection

_Methods_:

1. Correlation: Pearson, Point Bi-Serial, Cramer's V [reading materials](https://medium.com/@outside2SDs/an-overview-of-correlation-measures-between-categorical-and-continuous-variables-4c7f85610365)
2. Weight of Evidence and Information Value [reading materials](https://www.analyticsvidhya.com/blog/2021/06/understand-weight-of-evidence-and-information-value/)
3. Beta Coefficients [reading materials](https://www.statisticshowto.com/standardized-beta-coefficient/)
4. Lasso Regression [reading materials](https://machinelearningmastery.com/lasso-regression-with-python/)
5. Recursive Feature Selection [reading materials](https://scikit-learn.org/stable/modules/feature_selection.html#rfe)
6. Sequential Feature Selector [reading materials](https://scikit-learn.org/stable/modules/feature_selection.html#sequential-feature-selection)
7. BorutaPy [reading materials](https://github.com/scikit-learn-contrib/boruta_py)
8. BorutaShap [reading materials](https://medium.com/analytics-vidhya/is-this-the-best-feature-selection-algorithm-borutashap-8bc238aa1677)

_Features selected by majority of the methods will be picked for modelling.Users can select all methods or a subset of them_



## Data

_We are using the [(default of credit card clients)](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients) data. It has 30,000 records on customer default payments in Taiwan and has 23 features_:

1. Amount of the given credit (NT dollar): it includes both the individual consumer credit and his/her family (supplementary) credit.
2. Gender (1 = male; 2 = female).
3. Education (1 = graduate school; 2 = university; 3 = high school; 4 = others).
4. Marital status (1 = married; 2 = single; 3 = others).
5. Age (year).
6. History of past payment. We tracked the past monthly payment records (from April to September, 2005) as follows: X6 = the repayment status in September, 2005; X7 = the repayment status in August, 2005; . . .;X11 = the repayment status in April, 2005. The measurement scale for the repayment status is: -1 = pay duly; 1 = payment delay for one month; 2 = payment delay for two months; . . .; 8 = payment delay for eight months; 9 = payment delay for nine months and above.
7. Amount of bill statement (NT dollar). X12 = amount of bill statement in September, 2005; X13 = amount of bill statement in August, 2005; . . .; X17 = amount of bill statement in April, 2005.
8. Amount of previous payment (NT dollar). X18 = amount paid in September, 2005; X19 = amount paid in August, 2005; . . .;X23 = amount paid in April, 2005.


## Instructions

Users need to update the manual inputs section and the rest of the notebook should run smoothly




