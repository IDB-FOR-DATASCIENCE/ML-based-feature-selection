Feature Selection - Classification
Code Pipeline for using multiple feature selection methods for classification purpose

Contents
Purpose
Steps
Data
Instructions
Purpose:
This notebook is a one stop shop for ML based feature selection for classification purpose. Once the master data is prepared, we can use this notebook to try out 8 feature selection techniques and combine their results

Steps:
Step 1: Load Package and Custom Functions
Install/Import necesarry packages
Load custom functions
Input user defined metrics
Step 2: Data Preparation:
Import dataset
Profiling and EDA
Drop unwanted fields and convert column types
Null Treatment
Treating categorical features (one hot encoding, WOE encoding)
Train/Test/OOT Split
Step 3: Feature Selection
Methods:

Correlation: Pearson, Point Bi-Serial, Cramer's V reading materials
Weight of Evidence and Information Value reading materials
Beta Coefficients reading materials
Lasso Regression reading materials
Recursive Feature Selection reading materials
Sequential Feature Selector reading materials
BorutaPy reading materials
BorutaShap reading materials
Features selected by majority of the methods will be picked for modelling.Users can select all methods or a subset of them

Data
We are using the (default of credit card clients) data. It has 30,000 records on customer default payments in Taiwan and has 23 features:

Amount of the given credit (NT dollar): it includes both the individual consumer credit and his/her family (supplementary) credit.
Gender (1 = male; 2 = female).
Education (1 = graduate school; 2 = university; 3 = high school; 4 = others).
Marital status (1 = married; 2 = single; 3 = others).
Age (year).
History of past payment. We tracked the past monthly payment records (from April to September, 2005) as follows: X6 = the repayment status in September, 2005; X7 = the repayment status in August, 2005; . . .;X11 = the repayment status in April, 2005. The measurement scale for the repayment status is: -1 = pay duly; 1 = payment delay for one month; 2 = payment delay for two months; . . .; 8 = payment delay for eight months; 9 = payment delay for nine months and above.
Amount of bill statement (NT dollar). X12 = amount of bill statement in September, 2005; X13 = amount of bill statement in August, 2005; . . .; X17 = amount of bill statement in April, 2005.
Amount of previous payment (NT dollar). X18 = amount paid in September, 2005; X19 = amount paid in August, 2005; . . .;X23 = amount paid in April, 2005.
Instructions
Users need to update the manual inputs section and the rest of the notebook should run smoothly
