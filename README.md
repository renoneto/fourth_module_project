# Movie Recommender :clapper:

In this project, I'm creating a movie recommender model using the [MovieLens dataset](https://grouplens.org/datasets/movielens/) and deploying it. You can find more information about the model in the [Jupyter notebook](https://github.com/renoneto/fourth_module_project/blob/main/Movie%20Recommender.ipynb) and [you can see the app by clicking here](https://movie-recommender-reno.herokuapp.com/).

## Business Case and Goal

I was hired to create a model to provide 5 movie recommendations to users and I need to deal with the **cold start** problem (when it's a brand new user with no ratings in the database).

## The Dataset

The MovieLens dataset is a "classic" recommendation system dataset used in numerous academic papers and machine learning proofs-of-concept.

## Modeling

For modeling, I have attempted to use four different algorithms: Singular Value Decomposition (SVD), SVD++ , KNN Basic (A basic collaborative filtering algorithm) and KNN Baseline (A basic collaborative filtering algorithm taking into account a baseline rating.

Using `GridSearchCV` I fine tuned the SVD model and used the same hyperparameters for the SVD++ model.

For the KNN models, I have also tried different hyperparameter configurations.

### Result

In the end, the SVD model performed better (low RMSE with no indication of overfitting) with a low fit time relative to SVD++.

## App

To create the app I have used [Streamlit](https://docs.streamlit.io/en/stable/index.html) which is an open-source Python library that makes it easy to create and share beautiful, custom web apps for machine learning and data science.

I'm also deploying the model using Heroku. To make this all work I have different files in the same repository
