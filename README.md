# Movies-ETL by Alec Ngai

## Project Overview
We are tasked with creating datasets for a hackingathon, the client "Amazing Prime" wants a dataset that is always up to date and is automated in such a way that we extract, transform and load the dataset into a clean workable dataset. We do this in four tasks:

1. write an ETL function to read three data files,
2. extract and transform the Wikipedia data,
3. extract and transform the Kaggle and rating data,
4. load the data to a PostgreSQL Movie Database.

## Resources
- Data Source: movies_metadata.csv, ratings.csv, wikipedia-movies.json
- Software: Python 3.9.4, Visual Studio Code, 1.58.1, Conda 4.10.1, PostgreSQL 13.4, pgAdmin4 5.2

## Results

### Write an ETL function to read three data files
The function takes the Wikipedia JSON, the Kaggle metadata and MovieLens csv files and creates three separate DataFrames.
<br/>

### Extract and Transform the Wikipedia data
We filtered out the TV shows, consolidated the redundant data, removed the duplicates and formatted the Wikipedia data.
<br/>

### Extract and Transform the Kaggle and rating data
Again, we consolidated the redundant data, removed the duplicates, formatted and grouped the data.\
The Kaggle and rating data were then merged with the Wikipedia movies DataFrame.

### Load the data to a PostgreSQL Movie Database
<br/>
<p align="center">
  <img src="https://raw.githubusercontent.com/alecngai/08_Movies_ETL/main/Resources/movies_query.png"> 
</p>
<p align="center">
  <img src="https://raw.githubusercontent.com/alecngai/08_Movies_ETL/main/Resources/ratings_query.png"> 
</p>
<br/>

## Summary
The ETL function created collects and cleans movie data from different sources (Wikipedia JSON and Kaggle and ratings csv files). It transforms and merges the data and loads it into two updatable PostgreSQL dataset tables ready to be used by the hackathon participants for their analysis.