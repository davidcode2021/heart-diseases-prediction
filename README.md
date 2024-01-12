# heart-diseases-prediction  
# Content
feature engineering: in this part the data was prepared for fitting into the algorithm  
X; Features of the prepared data  
y: Target  
Searching_for_model:in this part the prepared data is fit into the 3 models and accuracy for each model was tested  
Heart.csv; this the data used for model
# Description  
in this project, a model is created using machine learning to predict whether a person will be down with heart diseases given some certain features.  
# Data  
the data for this project consist of 918 rows and 12 columns. The columns are Age, Sex, ChestPainType,RestingBP, Cholestoral, FastingBP, RestingECG, ExerciseAnina
OldPeak, ST_slope, heartDisease. The heartDisease is the target (dependent variable,y) while the rest are the features (independent variable,X). In the heartDisease 
column the value 1 means the person have heartDisease while 0 means he does not have heartDisease  
# Procedure  
All the outliers in the data was removed using Z score and replaced with their mean values. Duplicate values was checked. All the categorical non-numerical colums were one-hot encoded and scaled using standard save for the target column. Using principle component analysis the dimension of the data is reduce slighly. The data was split into features (X) and target(y). Using the K-fold validation (wih five folds) the accuracy of the model was tested  
The machine learning algorithm that was used are SVC, RandomforestClassifier and LogisticRegression  
# Result  
After testing the models. Random forest have the highest accuracy of 0.86  
# Acknowledgement  
The data for the project was gotten from kaggle.
