# Introduction
In this competition, hosted by IIT-KGP's KDAG (Kharagpur Data Analytics Group) we are tasked to create data science models to predict the customer attrition for a service based on data such as a customer's general bio-data, their payment history and subscriptions.

The details of the competition can be found here: [Kaggle](https://www.kaggle.com/c/customerattritionprediction/overview)

The Kaggle notebook can be found here: [Notebook](https://www.kaggle.com/rdev12/customer-attrition)

# Data
"ID", string, the Customer ID allocated to each customer,

"sex", string, the gender of the person,

"Aged", Boolean, tells if the person is old,

"Married", Boolean, The marrital status of the person,

"TotalDependents", Boolean, Tells whether the person is dependent or independent,

"ServiceSpan", numerical, gives the timespan of the service taken by the person,

"4GService",string, the intenet service taken by the person ,

"CyberProtection", Boolean, tells if cyber protection plan of company is taken by the person or not

"HardwareSupport", Boolean, tells if hardware support plan of company is taken by the person or not,

"TechnicalAssistance", Boolean, tells if technical assistance of company is taken by the person or not,,

"FilmSubscription", Boolean, tells whether the person has subscribed for films,

"SettlementProcess", string, The payment process chosen by the person,

"QuarterlyPayment", numerical, The quaterly payment made by the person,

"GrandPayment", numerical, The cummalative payment made by the person,

"CustomerAttrition", Boolean, The choice of continuation of services taken by the customer

# Dependencies
- numpy
- pandas
- seaborn
- matplotlib
- sklearn
- pandas_profiling

# Installation
  ```
  pip install numpy
  pip install pandas
  pip install seaborn
  pip install matplotlib
  pip install scikit-learn
  pip install pandas-profiling
  ```

# Model
Our model involves the stacking of
1. RandomForestClassifier
2. ExtraTreesClassifier
3. BalancedRandomForestClassifier

with Logistic Regression as the final estimator

# Results
The best submission (stack-sampled-classifier.csv) of our model performed with an accuracy of

0.83143 - Public Leaderboard

0.81355 - Private Leaderboard
