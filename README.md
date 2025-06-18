                                          Movie Recommendation System using SVD (Surprise Library)
This project implements a movie recommendation system using the Singular Value Decomposition (SVD) algorithm provided by the Surprise library. It uses the MovieLens dataset to predict user ratings and recommend top movies.

Dataset
The project uses the MovieLens small dataset, which contains:

ratings.csv with columns: userId, movieId, rating, timestamp

movies.csv with columns: movieId, title, genres

The dataset can be downloaded from https://grouplens.org/datasets/movielens/.

Requirements
Before running the code, install the following dependencies:

pip install numpy==1.24.4
pip install scikit-surprise
Note: scikit-surprise is not currently compatible with NumPy 2.x, so NumPy must be downgraded to version 1.24.4.

How to Run on Google Colab
Upload ratings.csv and movies.csv files to the Colab environment.

Install the required libraries.

Run the code cells step-by-step to train the model and view recommendations.

Features
Loads and prepares MovieLens data

Applies SVD-based collaborative filtering

Splits data into training and test sets

Predicts ratings for unrated movies

Recommends top 10 movies for a specified user

Evaluates model performance using RMSE

Model Used
The model used is the SVD (Singular Value Decomposition) algorithm, which is widely used for collaborative filtering in recommendation systems. It works by decomposing the user-item interaction matrix and estimating missing ratings.

Output
The system outputs the top 10 movie recommendations for a specific user (default is user ID 1), sorted by predicted rating. It also prints the RMSE value to indicate model accuracy.

