# Databricks_movie_recommendation_system

## Movies and Ratings dataset

Source: (movies.csv, ratings.csv) downloaded from kaggle
- https://www.kaggle.com/datasets/parasharmanas/movie-recommendation-system

## IMPLEMENTATION
- Extracted a separate delta table from dbfs file upload
- Trained a model using a MLflow run (ALS - for collaborative filtering)
- Saved model (to enable future re-training of ALS with additional data if needed)
- Generated Top-N recommendations from the trained model
- Saved the recommendations as a delta table (allowing possible streaming or processing later)

## Screenshots

### Resource Visualizer
![Upload Resource Visualizer (Screenshot)](Resource%20Visualizer%20.png)

### Resources
![Upload Resources (Screenshot)](Resources%20.png)

### Compute
![Upload Compute (Screenshot)](Compute%20.png)

### Upload to dbfs (data ingestion)
![Upload to dbfs (data ingestion) (Screenshot)](Upload%20to%20dbfs%20(data%20ingestion)%20.png)

### Data Ingestion (movies.csv)
![Upload Data Ingestion (movies.csv) (Screenshot)](Data%20Ingestion%20(movies.csv%20from%20local%20to%20DBFS)%20.png)

### Data Ingestion (ratings.csv)
![Upload Data Ingestion (ratings.csv) (Screenshot)](Data%20Ingestion%20(ratings.csv%20from%20local%20to%20DBFS)%20.png)

### Trying to read data from temp upload
![Upload Trying to read data (Screenshot)](Trying%20to%20read%20data%20from%20temp%20upload%20.png)

### Training the model
![Upload Training the model (Screenshot)](Training%20the%20model%20.png)

### ML flow run to an Experiment in MLFlow
![Upload MLflow run (Screenshot)](ML%20flow%20run%20to%20an%20Experiment%20in%20MLFlow%20.png)

### Saving the model and running the reccomendForAllUsers to get Top-N recommendations
![Upload Model run to get Top-N (Screenshot)](Saving%20the%20model%20and%20running%20the%20reccomendForAllUsers%20to%20get%20Top-N%20recommendations%20.png)

### Flattening the nested recommendations array and joining movie names
![Upload Flattening the nested rec. (Screenshot)](Flattening%20the%20nested%20recommendations%20array%20and%20joining%20movie%20names%20.png)

### Filtering out the movies that are already watched by a user
![Upload Filtering new rec. out (Screenshot)](Filtering%20out%20the%20movies%20that%20are%20already%20watched%20by%20a%20user%20.png)

### Saving the recommendations as a delta table
![Upload Saving the rec. to delta (Screenshot)](Saving%20the%20recommendations%20as%20a%20delta%20table%20.png)

### Freeing resources (Databricks)
![Upload Freeing resources (Databricks) (Screenshot)](freeing%20the%20resources%20.png)

### Freeing resources (Compute)
![Upload Freeing resources (Compute) (Screenshot)](freeing%20the%20resources%20(1)%20.png)
