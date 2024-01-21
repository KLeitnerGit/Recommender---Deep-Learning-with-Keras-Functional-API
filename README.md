# Recommender---Deep-Learning-with-Keras-Functional-API

## Project Overview

The "Recommender - Deep Learning with Keras Functional API" project is a deep learning-based approach to building a music recommendation system. The project leverages a subset of a comprehensive dataset from the Deezer Streaming Service, as provided in the Deezer Streaming Songs User Analytics Competition on Kaggle https://www.kaggle.com/c/dsg17-online-phase/overview.

## Objective
The primary objective of this project is to predict whether users of the Deezer app will listen to a given song for at least 30 seconds. This binary classification problem (is_listened = 1 if listened for over 30 seconds, otherwise 0) aims to model user preferences and enhance the listening experience by recommending tracks that align with their tastes.


## Data Preprocessing

A 1% random sample of the original dataset is used due to computational constraints. The dataset includes various features like user ID, media ID, genre ID, context type, and the target variable is_listened.

## Model Architecture

Two baseline models are developed:

Collaborative Filtering Model: Uses user and media embeddings.
Hybrid Model: Incorporates context type along with user and media embeddings.
Both models are implemented using the Keras Functional API, allowing for flexible model architectures and the integration of different data types.

## Training and Evaluation

The models are trained on 80% of the data and tested on the remaining 20%. Performance metrics such as accuracy, precision, recall, and F1-score are used to evaluate the models.

## Results

The Collaborative Filtering Model showed an accuracy of approximately 70% on the test set.
The Hybrid Model, which also includes context type, achieved an accuracy of around 71%.

These baseline models provide a starting point for building more complex recommendation systems. Future improvements could include more sophisticated feature engineering, hyperparameter tuning, and the incorporation of additional data sources.
