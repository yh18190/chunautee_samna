# chunautee_samna
This repository is based on churn prediction problem of a platform.

Notebooks:
1.DataPrep_Transformations.ipynb : The code is used to for analysing,cleaning and transform the data for generating training dataset (binary classification imbalance problem).

2.ExploratoryDataAnalysis.ipynb : It contains visualizations of relationships between the data attributes for analysis.

3.Modelling.ipynb : The entire modelling of training data is part of the code.Have tried 5 different models including hyperparameter tuning and cross-validation techniques.

Algorithms used:
1.Logistic Regression
2.Random forest classifier
3.LightGBM Classifier
4.Xgboost Classifier
5.LightGBM -Hyperparamter Tuned(few parameters only because of time constraints etc)


Libraries :
1.Sklearn - ML libraries
2.Pandas,Numpy - Data Preprocessing and Transformations
3.Matplotlib,Plotly,Seaborn -Visualization
4.Hyperopt - Hyperparamter optimisation
5.Yellowbricks Classifier mainly for Discrimination Threshold: Shows precision, recall, f1, and queue rate over all thresholds for binary classifiers that use a discrimination probability or score.
6.Pickle 


Evaluation metrics considered across models:
1.F1-score
2.Roc-AUC score
3.Accuracy
4.Kappa score
5.Recall-score & Precision score


Areas of Improvements:
1.Hyperparamter Tuning using Gridsearch/RandomsearchCV and other tuning techniques to be implemented

2.Using H2oAutoML for modelling .as it does stacking and ensemble of multiple models together for better accuracy and its proven in many cases

3.Customer segmentation((new or existing users)/ (spenders vs non-spenders) by considering there tenure in the platform(how long they have been using and registration info,demographics info etc) could augment data and improve modelling.As we have seen the (number_of_daysbefore_lastdate) and diff_days_between_first_last_order features capture some of this essence.

4.Deep learning like sequence modelling(RNN) could be used be tried

5.Rating or Estimated_delivery_time etc attributes could also add value to add to understand customers sentiment towards orders.

6.As part of feature engineering ,some complex Feature transformations could be used like log,exponential for numerical values especially (amount_paid_sum,delivery_fee_sum etc).

7.Sometimes the failed ones are happening immediately before the successful one.Further analysis is needed whether to retain this info or exclude etc.it could also happen because of restaurants platform issues.

8.Handling missing data with Smote and other data imputation techniques..we can also try to use imblearn for handling class imbalances .Some outliers would need further investigation to understand the source of error.

9.Recursive Feature elimination,Anova and other feature selection techniques can be tried for reducing the feature space etc.

10. Using SHAP,LIME or explainx libraries for model interpretation could help build trustable model. 

