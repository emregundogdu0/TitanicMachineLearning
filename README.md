Titanic Survival Prediction

A machine learning deployment to forecast the survival of Titanic passengers using Random Forest classification. Project Overview This project explores the widely used Titanic dataset with the aim of developing a prediction model that forecasts whether a passenger survived the disaster. The model provides predictions based on passenger characteristics such as class, gender, age, and relationships. Dataset
The original Titanic dataset is what the project employs, having information on passengers aboard the RMS Titanic. The information consists of:

Training data: This is employed in training the machine learning model Test data: This is used to make a prediction for testing

-Features Used

Pclass: Passenger class (1st, 2nd, 3rd) Sex: Gender of the passenger Age: Age of the passenger SibSp: Siblings/spouse on board Number Parch: Parents/children on board Number Fare: Passenger fare Embarked: Port of embarkation (S = Southampton, C = Cherbourg, Q = Queenstown)

-Data Preprocessing

Missing data is handled by the model by means of a variety of strategies:

Age: Replaced missing values with median age Embarked: Replaced missing values with mode of most common port Fare: Replaced missing values with median fare Categorical encoding:
Sex: 0=male, 1=female Embarked: 0=S, 1=C, 2=Q

-Model Details

Algorithm: Random Forest Classifier Parameters: 100 estimators, random_state=42 Features: 7 numeric features after preprocessing Target: Binary classification (0=Did not survive, 1=Survived)

-Running the Model

Ensure you possess training data (train.csv) and test data (test.csv) in the same folder Run the Jupyter notebook titanic.ipynb The model will make predictions and save them in predictions.csv

-Results

The model predicts for 418 test passengers and prints them in the right format: csvPassengerId,Survived 892,0 893,0 894,0 .

-Key Insights

Survival was influenced by the following from the Titanic dataset:

Gender: Women were more likely to survive Passenger Class: First-class travelers were more likely to survive Age: Children and younger travelers were more likely to survive Family Size: Small-family passengers were more likely to survive compared to solo passengers or passengers with large families
