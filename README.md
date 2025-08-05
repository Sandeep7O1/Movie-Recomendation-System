# Movie-Recomendation-System

A simple movie recommendation system built using Python and the MovieLens 100K dataset. This project uses collaborative filtering based on user similarity and correlation to recommend movies similar to a given title.

# Features
Data preprocessing and merging of rating data with movie titles

Exploratory Data Analysis (EDA) using Seaborn & Matplotlib

Visualization of movie popularity and rating distributions

Creation of user-movie pivot table

Movie similarity calculation using Pearson correlation

Filter recommendations based on the number of ratings for better accuracy


# Dataset
Ratings file: u.data (tab-separated)

Movie titles file: Movie_Id_Titles.txt

Source: MovieLens 100K dataset

# Libraries Used
pandas

numpy

matplotlib

seaborn

# Recommendation Logic
A user-movie matrix is created with users as rows and movies as columns.

For a target movie (e.g., "Star Wars"), we extract its user rating vector.

We compute the correlation between this vector and every other movie.

Movies with high correlation scores and a sufficient number of ratings are considered most similar and recommended.
