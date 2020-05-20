# Predict-IMDB-rating-of-a-movie

### The report: Predict IMDB rating of a movie Lei Jiang Report.pdf
### The main notebook is Predict IMDB rating of a movie_fullFeatures-XGBbase.ipynb
#### It contains a write up summary of this project and most data preparation and EDA are in this notebook. There are other notebooks in this repo that contain other types of models.

### Target: predict imdb_score, regression problem.

#### There are four types of models I built - XGB, LGB, MLP, MLR. 
#### To make sure the models are comparable, all models are built on the same train and test datasets.
####  best model of each type - RMSE on test dataset

| Model Name  |    Root Mean Squared Error      | 
|-------------|---------------|
| XGB         |      0.7566          |  
| LGB         |   0.7354    |  
| MLP |            1.1672   |
| Multiple Linear Regression |  0.8925  |   

Table. Model RMSE Comparsion and Evaluation

### Conclusion
The best model I would choose for deployment is LGB which has the best test RMSE after hyper-parameters tuning as well as the second fastest training time.
