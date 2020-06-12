# Predict-IMDB-rating-of-a-movie

### Goal: 
build machine learning models to predict the IMDb score based on a variety of attributes of movies, compare the model performances and pick the best model for deployment.

#### Data source:
https://github.com/sundeepblue/movie_rating_prediction/


### Method
Feature engineering with NLP features; hyperparameters tuning for XGB,LGB; Neural Architecture Search for MLP.


### Target: 
predict imdb_score, regression problem.

#### There are four types of models I built - XGB, LGB, MLP, MLR. 
#### To make sure the models are comparable, all models are built on the same train and test datasets.
### Model performance - test RMSE and Training Time 
#### -best model of each type

| Model Name  |    Root Mean Squared Error      | Training Time|
|-------------|---------------|------------------------|
| XGB         |      0.7566          | 38.1 s  |
| LGB         |   0.7354    |  24.3 s    |  
| MLP |            1.1672   | 3min 25s   |
| Multiple Linear Regression |  0.8925  |    2.46 ms  |  

### Conclusions
Based on the Model performance considering RMSE and Training Time, the best model I would choose for deployment is LGB which has the best test RMSE after hyper-parameters tuning as well as the second fastest training time.

The decision also depends on the requirement of deployment, if we deploy the model on the edge like wearable devices or smart phones where the computation power is limited and the prediction accuracy is not critical, we may also deploy a simpler model like MLR since it requires very little computation power and run extremely fast (2.46 ms).


### The report: 
"Predict IMDB rating of a movie Lei Jiang Report.pdf"

### The main notebook：
"Predict IMDB rating of a movie_fullFeatures-XGBbase.ipynb"
#### It contains a write up summary of this project and most data preparation and EDA are in this notebook. There are other notebooks in this repo that contain other types of models.
