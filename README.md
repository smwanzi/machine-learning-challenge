##  **Machine Learning Homework - Exoplanet Exploration**

Over a period of nine years in deep space, the NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets outside of our solar system.

The assignment is to create machine learning models capable of classifying candidate exoplanets from the raw dataset.

## Instructions 

### Preprocess the Data

-Preprocess the dataset prior to fitting the model.
-Perform feature selection and remove unnecessary features.
-Use MinMaxScaler to scale the numerical data.
-Separate the data into training and testing data.

### Tune Model Parameters

-Use GridSearch to tune model parameters.
-Tune and compare at least two different classifiers.

### Reporting

Create a README that reports a comparison of each model's performance as well as a summary about your findings and any assumptions you can make based on your model (is your model good enough to predict new exoplanets? Why or why not? What would make your model be better at predicting new exoplanets?).


## Analysis

### Model-1 SVM

-The data was scaled and normalized to reduce the gap between data points in order to have acurate weights for the model. 
-Used MinMaxScaler to scale the data with SVM model, the returned scores were; Training Data Score: 0.85 and 
Testing Data Score: 0.84.

-Using GridSearchCV to tune the model's parameters returned slightly higher scores of; Training Data Score: 0.871 ,Test Data: 0.874


### Model-2 Logistic Regression

-Used the StandardScaler to scale and normalize the data.
-The scores for training and testing data was :Training Data Score: 0.887659736791913, Testing Data Score: 0.8895881006864989.
-Using GridSearchCV to tune the model's parameters, and changing C values, and increasing the number of iterations max_iter didn't improve scores sufficiently.

In Summary, the two models SVM and LogisticRegression didn't have any significant difference between them for this data, even hyperparameters tuning didn't help to differentiate the models significantly. However, the SVM model had  an accuracy of .99f1-score while the Logistic Regression model had an accuracy of .88 f1-score, making the SVM model slightly better than the Logistic Models.


© 2020 GitHub, Inc.
Terms
