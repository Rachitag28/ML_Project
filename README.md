# ML_Project
## Machine Learning project - University of Cincinnati

## AIM

#### The aim of the project is to build a Hybrid Recommender System to recommend movies by learning behaivor of each user. Hybrid Recommender System combines the advantages of both Collaborative Filtering and COntent Based Filtering.

## Dataset

#### Data used for this model is the combination of data from Movielense Data (ml-latest-small) and Scrapped data from IMDB

## Collaborative Filtering

#### In Collaborative Filtering similar users that have similar preference values for similar movies are clustered together. For a specific user, a fixed number of users that have provided most similar rating for the movies rated by that specific user are included in the cluster of similar users.
#### It is assumed that users having similar preference in the past tends to have similar preference in future.
#### K-Nearest Neighbors classification was used to form cluster of similar users in this model.

## Content - Based Filtering

#### In this method information about movies are analysed and based on that a cluster of most similar movies is formed. DIfferent attributes of movies such as Casting, Director, Genre etc. are used as features and the movies with most similar features are clustered together.
#### Movies rated by a specific user are considered to determine the most similar movies from the list of movies.
#### K-Nearest Neighbor was implemented to cluster the most similar movies based on their attribute set.

## Recommendations

#### For a specific user, Users form the cluster of most similar users (formed using collaborative filtering) and movies from the most similar movie cluster (formed using content-based filtering) are considered together. The most similar movies which are rated highes by the most similar users are provided as the final recommendations for a specific user. Along with the recommendations an estimated rating is also provided which is basically a expected rating value that the user will provide for recommended movies.

