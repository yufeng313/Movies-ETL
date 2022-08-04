# Movies-ETL
Using ETL process to creat data pipelines
## Overview
The Amazing Prime video team would like to develop an algorithm to predict which low budget movies being released will become popular, so we will need to create an automated pipeline that takes in all the movie data, performs the appropriate transformations, and loads the data into SQL tables.
In this challenge, we are going to create a function that takes in the three files—Wikipedia data, Kaggle metadata, and the MovieLens rating data—and performs the ETL process by adding the data to a PostgreSQL database. 

## Resources
Data source: wikipedia-movies.json, movies_metadata.csv, ratings.csv <br/>
Software: Postgresql 11.16,   Pgadmin4 6.11,  Python 3.7.6,   Jupyter Notebook 6.4.8

## Results
### Deliverable 1: Write an ETL Function to Read Three Data Files<br/>
Write a function that reads in the three files: Wikipedia JSON, the Kaggle metadata and MovieLens ratings CSV files, and creates three separate DataFrames.<br/>
![Screen Shot 2022-08-03 at 9 36 01 PM](https://user-images.githubusercontent.com/107179765/182764187-35ad4e82-be45-443e-8ad2-77b7e8dcd944.png)

### Deliverable 2: Extract and Transform the Wikipedia Data<br/>
Create a clean_movie function to handle the alternative titles, filter out the TV shows, extract the IMDb IDs using a regular expression string and drop duplicates of the Wikipedia data.<br/>

### Deliverable 3: Extract and Transform the Kaggle data<br/>
Extract and transform the Kaggle metadata and MovieLens rating data. Then, merge the Kaggle metadata DataFrame with the Wikipedia movies DataFrame to create the movies_df DataFrame, again, remove the duplicates and format the data. Finally, merge the MovieLens rating data DataFrame with the movies_df DataFrame to create the movies_with_ratings_df.<br/>

### Deliverable 4: Create the Movie Database<br/>
Add the movies_df DataFrame and MovieLens rating CSV data to the SQL database.<br/>
![Screen Shot 2022-08-03 at 9 18 39 PM](https://user-images.githubusercontent.com/107179765/182763412-0b12f810-5404-4f1e-ba40-ae9f3c605c79.png)

## Summary
![data-8-1-1-1-extract-transform-load](https://user-images.githubusercontent.com/107179765/182763460-2df7fc37-53fd-4c86-84b9-e32a158c712d.png)
The ETL function create collects and cleans movie data from different sources (Wikipedia JSON and Kaggle and ratings csv files). It transforms and merges the data and loads it into two updatable PostgreSQL dataset tables ready to be used by the hackathon participants for their analysis.
