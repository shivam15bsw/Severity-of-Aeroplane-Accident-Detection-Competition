# Severity of Aeroplant Accident Detection
Machine Learning model to detect Severity of Airplane Accident 


How severe can an airplane accident be?




Initially various models were trained to select the best model. Gradient Boosting Classifier came out to be the best model for this Classification Model. 


On the Basic of Feature Importance of Gradient Boosting Classifier 7 features (Violations, Total_Safety_Complaints, Cabin_Temperature, Max_Elevation, Adverse_Weather_Metric, Turbulence_In_gforces, Accident_Type_Code) were removed because then the accuracy was best on Whole training Set i.e. approx. 99.96 % on the Training Data.


Initially some feature engineering like the number of NULL values checking, plots,  converting strings of outputs to numbers etc were done. Then several models like:
* Logistic Regression
* SVM
* Decision Trees 
* Random Forest Classifier
* Gradient Boosting Classifier
* Neural Networks
were trained to select the best model on the basis of f_1 score on the test Data obtained from train test split. Then the Gradient Boosting Classifier model had the best f_1 score so it was finally trained to select top 3 features and also hyper[parameters tuning were done to ensure that the model is not overfitting and generating the best Data.


Parameters used for the Final Gradient Boosting Model:
* n_estimators = 2,000
* max_depth=4
* learning_rate=0.1 
* And rest default values.


After the training and testing on the train test split data model was trained on the whole Data Set so that we can use more data for the training of the model. After which test data was imported to do final predictions and was saved in an excel sheet.
