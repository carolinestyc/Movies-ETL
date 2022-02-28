# Movies-ETL
  Challenge 8

## Project Overview
Amazing Prime wants to know what movies will be popular soon so they can buy the streaming rights ahead of time. They have decided to hold a Hackathon so the community can help with the project. We have created and cleaned the database by combining a Wikipedia Source, a Kaggle Source, and MovieLens rating data to use in the hackathon. Now, they want the database to have an automatic pipeline to bring in new data, perform the appropriate transformations, and load the data into existing tables. I have created a code that uses the ETL process to add the updated data to tables in PostgreSQL. 

### Resources
            Data Sources: ratings.csv, movies_metadata.csv, wikipedia-movies.json
            
            Software: Jupyter Notebook, PostgreSQL, & pgAdmin 4
            
## Findings
In order to load the transformed data to an SQL database, a connection had to be made to the server. After the connection is made and the data is begins to upload, the time elapsed in seconds is counted to give us an idea of how long the databse update takes. In the image below you can see it took a long time for the over 26 million rows to upload to the database. Informing us that every time one wants to update the database, there will be significant time lapse to do so. 

![time_elapsed](https://user-images.githubusercontent.com/96352625/155919419-d8639db8-07df-498f-a18a-13405985ce69.png)

After extracting and transforming the data, we develop two (2) tables to load to pgAdmin. First, a movies table that has all movies released since 1980. A quick query of the table shows us there are 6,052 movies in the database.

<img width="341" alt="movies_query" src="https://user-images.githubusercontent.com/96352625/155920139-23ae14a0-112e-48eb-99a7-78b0e4bde4bf.png">


Second, a ratings table. A comprehensive list of ratings for these 6,052 movies from MovieLens, totalling 26,024,289 rows.

<img width="347" alt="ratings_query" src="https://user-images.githubusercontent.com/96352625/155920148-23657722-e930-420c-bd95-5550ea3507c5.png">



## Summary
