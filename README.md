# A-collaborative-Movie-Recommender-System


## Project Summary ##
This project implements a hybrid movie recommender system using data from the MovieLens dataset. The primary approach is collaborative filtering using item-item similarity (K-Nearest Neighbors), enhanced with content-based filtering to address the cold start problem.
The goal is to find/suggest similar movies to users based on past ratings, utilising techniques like Bayesian averaging for popularity estimation, matrix factorisation (SVD) for dimensionality reduction, and fuzzy matching for user input flexibility.


## Tools & Libraries ##
- Python
- Numpy
- Pandas
- Matplotlib & Seaborn
- Scikit-Learn
- FuzzyWuzzy
- MovieLens Dataset


## Project Overview ##

### Data Acquisition ###

- Movie ratings and metadata from the MovieLens dataset (ratings.csv, movies.csv).

### Exploratory Data Analysis (EDA) ###

- Distribution of ratings

- ovie popularity analysis using Bayesian average rating

### Data Preprocessing ###

- Created mapping dictionaries for user/movie IDs and titles

- Constructed a utility matrix (users × movies)

- Evaluated matrix sparsity

### Collaborative Filtering ###

- Implemented item-item similarity using K-Nearest Neighbors

- Built a function to recommend movies similar to a given title based on user ratings

### Cold Start Handling (Content-Based Filtering) ###

- Converted movie genres into binary feature vectors

- Used genre similarity to recommend movies when rating data is unavailable

- Integrated fuzzy string matching (fuzzywuzzy) for flexible user input

### Dimensionality Reduction ###

- Applied Singular Value Decomposition (SVD) for matrix factorisation
