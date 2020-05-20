# Predict-IMDB-rating-of-a-movie

### The report: Predict IMDB rating of a movie Lei Jiang Report.pdf
### The main notebook is Predict IMDB rating of a movie_fullFeatures-XGBbase.ipynb
#### It contains a write up summary of this project and most data preparation and EDA are in this notebook. There are other notebooks in this repo that contain other types of models.

### Target: predict imdb_score, regression problem.

#### There are four types of models I built - XGB, LGB, MLP, MLR. 
#### To make sure the models are comparable, all models are built on the same train and test datasets.
### Model performance RMSE and Training Time (best model of each type)

| Model Name  |    Root Mean Squared Error      | Training Time|
|-------------|---------------|------------------------|
| XGB         |      0.7566          | 38.1 s  |
| LGB         |   0.7354    |  24.3 s    |  
| MLP |            1.1672   | 3min 25s   |
| Multiple Linear Regression |  0.8925  |    2.46 ms  |  

### Conclusion
The best model I would choose for deployment is LGB which has the best test RMSE after hyper-parameters tuning as well as the second fastest training time.
