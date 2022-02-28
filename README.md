# Movies-ETL
  Challenge 8

## Project Overview
Amazing Prime wants to know what movies will be popular soon so they can buy the streaming rights ahead of time. They have decided to hold a Hackathon so the community can help with the project. We have created and cleaned the database by combining a Wikipedia Source, a Kaggle Source, and MovieLens rating data to use in the hackathon. Now, they want the database to have an automatic pipeline to bring in new data, perform the appropriate transformations, and load the data into existing tables. I have created a code that uses the ETL process to add the updated data to tables in PostgreSQL. 

### Resources
            Data Sources: ratings.csv, movies_metadata.csv, wikipedia-movies.json
            
            Software: Jupyter Notebook, PostgreSQL, & pgAdmin 4
            
## Findings
After exctracing and transforming the data, we develop two (2) tables. First, a movies table that has all movies released since 1980. A quick query of the table shows us there are 6,052 movies in the database.

<img width="347" alt="movies_query" src="https://user-images.githubusercontent.com/96352625/155919388-c8e9e3ef-c934-4631-aea8-080c88f390d4.png">

Second, a ratings table. A comprehensive list of ratings for these 6,052 movies from MovieLens, totalling 26,024,289 rows.

<img width="341" alt="ratings_query" src="https://user-images.githubusercontent.com/96352625/155919409-296e8f53-892f-4c70-8753-4648d39262be.png">

![time_elapsed](https://user-images.githubusercontent.com/96352625/155919419-d8639db8-07df-498f-a18a-13405985ce69.png)

## Summary
