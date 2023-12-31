# Bank_GoodCredit-Client-Project


## BUISNESS CASE :- 
Bank GoodCredit wants to predict cred score for current credit card customers. The cred score will denote a customer’s credit worthiness and help the bank in reducing credit default risk.

### INTRODUCTION OF PROJECT :-
 * A credit card is a financial instrument, which can be used more than once to borrow money or buy products and services on credit.
 * Banks, retail stores and other businesses generally issue these.

**Credit limit:-**
   * The maximum amount of charges a card holder may apply to the account.

**Annual Fee:-**
   * A bank charge for use of a credit card levied each year, which ranges depending upon the type of card one possesses.Banks usually take an initial 
  fixed amount in the first year and thena lower amount as yearly renewal fees. Revolving Line Of Credit

**TARGET COLUMN == Bad_label**
   * 0 Represent--Customer has Good credit history
   * 1 Represent--Customer has Bad credit history

### PROJECT GOAL :-

**Build a model with the data provided**
1. Data exploration insights – what did you find and what decision did you take?
2. Feature matrix - List of features selected with gain
3. Model evaluation - Gini and rank ordering

### PROJECT IS DEVICE INTO CERTAIN STEPS:
1. Featching data from data-base.
2. Domain analysis.
3. EDA: [Univariate, Bivariate & Multivariate analysis condition]
4. Data preprocessing/Feature Engineering.
5. Feature selection.
6. Model creation.
7. Model Evaluation.
8. Model Saving.

### DOMAIN ANALYSIS :-
#### Customer Account Data (Table : Cust_Account) :- 
   *  This table contains customer’s historical accounts data   and payments history.
#### Customer Enquiry Data (Table : Cust_Enquiry) :-
   * This table contains customer’s historical enquiry data   such as enquiry amount and enquiry purpose.
#### Demographics Data (Table : Cust_Demographics) :- 
   * Current customer applications with demographic data.

*  Note that demographics features are renamed as features and obscured in accordance with privacy policies.

### DATA SUMMARY :-
* In this data all types of datatype is available.
* In this data some feature are unique so we can not perform any analysis on this feature.
* In this data some feature contain blank spaces so we need to replace with NAN values.
* Not impute the outlier we are scaling to robust the outlier.
* Use Labal encoding technique to handle categorical feature.

### BASIC CHECKS :-
* In this data total 23896 observation with 92 feature.
* Some of unique feature in data
* One constant column in data.

### EXPLOTARY DATA ANALYSIS :-
**TARGET COLUMN ==Bad_label :-**
  * 0 Represent--> Customer has Good credit history.
  * 1 Represent--> Customer has Bad credit history.

 ![image](https://github.com/GaneshAhire30/Bank_GoodCredit-Client-Project/assets/114847888/dc7c6c2b-5795-4bee-8d28-88425466ff2e)
  
  * In this plot we are clearly seen the 90% Customer has Good credit and 10% customer are did not do has Good credit.
  * In this data we Not do any domain analysis because data is contain private information of customer details of Bank.

### DATA PREPROCESSING :-
* In this data set blank spaces are available so I converted to NaN values.
* In this data set most of the feature contain missing value with including unique feature.
  Numerical feature missing value impute with Median/Mean. And Categorical feature missing value impute with mode(use fillna function to impute categorical 
  value).
* Some Features has more than 15% to 90% missing value and some unique feature also contain missing value so we drop this feature.
* Handle categorical data using a Labal Encoding.
* Not impute the outlier we are scaling to robust the outlier.
* Robust scaler are robust to outlier. it is used to sacled the feature to median and quantile scaling.

### FEATURE ENGINEERING :-
* Drop all unique columns and Constant feature.
* Changing the data type.
* Get correlation and plot heat map.
* Their is no Duplicates present in data.

### SAVE PRE-PROCESS DATA :-
*	Save all pre-process data

### MODEL CREATION AND EVALUATION :-
* Logisticregression classifier model is well work on training data as well as testing data And The score of training and testing data is 74 %. But Testing accuracy is still lagging so i apply bagging. After apply bagging score is slightly improve(After bagging score = 77.76%).

* KNeighboursClassifier model is slightly perform well accuracy on training data as well as testing data. The score of training   and testing data with respect to 87.73% & 78.03% .Testing accuracy is still lagging so i apply bagging. but Score Not improve after bagging (Aftre bagging score = 76.86%.

* Decision Tree Classifeir model is very well work on training data and The score of training data is 100% .Testing data is also good and testing score is 93%.

* Random Forest Classifier model is also very well work on training data and The score of training data is 100% .Testing data is also good and testing score is 96.51%.

* Geadient Boosting Classifier model is good work on training and teasting data. it's score is also same like training score is 92.44% and testing score is 92.41%.

* XGB Classifier model is perform well accuracy on training data as well as testing data. The score of training and testing data with respect to 96.34% & 95.42% .

* ANN model not perform well on training as well as testing data.

### CONCLUSION :-
* From above all model Im select XGB classifier beacuse this model perform well on training as well as testing side and low variance and low bias model. 

### MODEL SAVING :-
* Save the model using pickle





                                                                    

