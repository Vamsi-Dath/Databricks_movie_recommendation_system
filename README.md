# Databricks_movie_recommendation_system

## Movies and Ratings dataset

Source: (movies.csv, ratings.csv) downloaded from kaggle
- https://www.kaggle.com/datasets/parasharmanas/movie-recommendation-system

## IMPLEMENTATION
- Extracted a sepearate delta table from dbfs file upload
- Trained a model using a MLflow run (ALS - for collaborative filtering)
- Saved model (to enable future re training of ALS with additional data if needed)
- Created Top-N recommendations from the trained model
- Saved the recommendations as a delta table (allowing possible streaming or processing later)
