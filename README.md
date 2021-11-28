# Flight-Fare-Prediction


**Motivation**
       
       
       What to do when you are at home due to this pandemic situation?
       I started to learn Machine Learning model to get most out of it. 
       I came to know mathematics behind all supervised models. 
       Finally it is important to work on problems (real world application) to actually make a difference.



** Data Collection**

        Data Source - Kaggle Link - https://www.kaggle.com/nikhilmittal/flight-fare-prediction-mh/
            
            
            
            
**Importing dataset**


         1.Since data is in form of excel file we have to use pandas read_excel to load the data

         2.After loading it is important to check the complete information of data as it can indication many of the hidden infomation such as null values in a column or a row

         3.Check whether any null values are there or not. if it is present then following can be done, Imputing data using Imputation method in sklearn

         4.Filling NaN values with mean, median and mode using fillna() method

         5.Describe data --> which can give statistical analysis
         
         
         
**EDA**
         From description we can see that Date_of_Journey is a object data type,\ Therefore, we have to convert this datatype into timestamp so as to use this column properly for prediction

         For this we require pandas to_datetime to convert object data type to datetime dtype.

         **.dt.day** method will extract only day of that date

         **.dt.month** method will extract only month of that date
         
         
         
         
**Handling Categorical Data**

          One can find many ways to handle categorical data. Some of them categorical data are,

          Nominal data --> data are not in any order --> OneHotEncoder is used in this case

          Ordinal data --> data are in order --> LabelEncoder is used in this case





**Feature Selection**

          Finding out the best feature which will contribute and have good relation with target variable. Following are some of the feature selection methods,

          **1.heatmap**

          **2.featureimportance**

          **3.SelectKBest**
          
          
        
        
        
 **Fitting model using Random Forest**
 
 
 **Hyperparameter Tuning**
 
            1.Choose following method for hyperparameter tuning [RandomizedSearchCV --> Fast] /[ GridSearchCV]

            2.Assign hyperparameters in form of dictionery

            3.Fit the model

            4.Check best paramters and best score
