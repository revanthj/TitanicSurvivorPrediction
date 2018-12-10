# TitanicSurvivorPrediction

Data Source : Kaggle

The sinking of the RMS Titanic is one of the most infamous shipwrecks in history.  On April 15, 1912, during her maiden voyage, the Titanic sank after colliding with an iceberg, killing 1502 out of 2224 passengers and crew. 

In this challenge, it is asked to complete the analysis of what sorts of people were likely to survive. In particular, it is asked to apply the tools of machine learning to predict which passengers survived the tragedy.

  - [Exploratory Data Analysis](#exploratory-data-analysis)
  - [Logistic Regression](#logistic-regression)
  - [Kfold CV Logistic Regression](#kfold-cv-logistic-regression)
  - [Decision Tree Model](#decision-tree-model)
  - [Random Forest Model](#random-forest-model)
  - [K Nearest Neighbors Model](#k-nearest-neighbors-model)
  - [Support Vector Model](#support-vector-model)
    
  
## Exploratory Data Analysis

**Notebook :** ExploratoryDataAnalysis.ipynb

**Key Steps:**
* Fill missing values for features by taking appropriate approach.

* Visualize distribution of survivors across features. Drop unwanted columns.

* Find coorelation between features.
  
* Apply Backward Elimination technique and select features that have significant impact on Survival rate.


## Logistic Regression

**Notebook :** LogisticRegression.ipynb

**Key Steps:**
* Impute missing values.

* Split input data into training and test sets. Train basic linear model with default parameters on training data and establish baseline scores.

* **SUMMARY**
  * Accuracy :  80.39%
  
  
## Kfold CV Logistic Regression

**Notebook :** KfoldCVLogisticRegression.ipynb

**Key Steps:**
* Impute missing values. Split input data into training and test sets.

* Find optimal value of regularization parameter (C) by training baseline linear model with different values and estimating accuracy of predictions

* Implement Logistic Regression with Stratified fold (Stratification is the process of rearranging the data as to ensure each fold is a good representative of the whole) CV approach and optimal value of regularization parameter. Compare model performance with that of basline.

* **SUMMARY**
  * Baseline Model Accuracy :  80.39%
  * Stratified Fold CV Model Accuracy : 83.24%
  
  
## Decision Tree Model

**Notebook :** DecisionTreeModel.ipynb

**Key Steps:**
* Impute missing values. Split input data into training and test sets.

* Train bsaeline model with default parameters and establish benchmark scores.  

* Implement Hyper Parameter tuning using RandomizedSearchCV and find optimal values.

* Implement model with optimal values and compare its performance with that of baseline model.

* Visualize Decision Tree using **StringIO and export_graphviz**

* **SUMMARY**
  * Baseline Model Accuracy :  81.00%
  * Optimal Parameter Model Accuracy : 82.12%
  
  
## Random Forest Model

**Notebook :** RandomForestModel.ipynb

**Key Steps:**
* Impute missing values. Split input data into training and test sets.

* Train bsaeline model with default parameters and establish benchmark scores.  

* Implement Hyper Parameter tuning using RandomizedSearchCV and find optimal values.

* Implement model with optimal values and compare its performance with that of baseline model.

* **SUMMARY**
  * Baseline Model Accuracy :  82.12%
  * Optimal Parameter Model Accuracy : 81.56%


## K Nearest Neighbors Model

**Notebook :** KNNModel.ipynb

**Key Steps:**
* Impute missing values. Split input data into training and test sets.

* Train bsaeline model with default parameters and establish benchmark scores.  

* Tune KNN model by changing n_neighbors. Select optimal value.

* Implement model with optimal values and compare its performance with that of baseline model.

* **SUMMARY**
  * KNN Baseline Model Accuracy :  79.32%
  * KNN Model with Manhattan distance metric and n_neighbors = 17 Accuracy  : 82.12%
  
  
## Support Vector Model

**Notebook :** SVMModel.ipynb

**Key Steps:**
* Impute missing values. Split input data into training and test sets.

* Train bsaeline model with default parameters and establish benchmark scores.  

* Implement Hyper Parameter tuning by using GridSearchCV and StratifiedKFold approach

* Implement model with optimal values and compare its performance with that of baseline model.

* **SUMMARY**
  * Baseline Model Accuracy :  83.24%
  * Optimal Parameter Model Accuracy  : 83.24%
