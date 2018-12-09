# TitanicSurvivorPrediction

Data Source : Kaggle

The sinking of the RMS Titanic is one of the most infamous shipwrecks in history.  On April 15, 1912, during her maiden voyage, the Titanic sank after colliding with an iceberg, killing 1502 out of 2224 passengers and crew. 

In this challenge, it is asked to complete the analysis of what sorts of people were likely to survive. In particular, it is asked to apply the tools of machine learning to predict which passengers survived the tragedy.

  - [Exploratory Data Analysis](#exploratory-data-analysis)
  - [Logistic Regression](#logistic-regression)
    
  
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
