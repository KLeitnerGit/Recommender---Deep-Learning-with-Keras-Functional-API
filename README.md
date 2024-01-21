# Recommender---Deep-Learning-with-Keras-Functional-API

## Project Overview

The "Recommender - Deep Learning with Keras Functional API" project is a deep learning-based approach to building a music recommendation system. The project leverages a subset of a comprehensive dataset from the Deezer Streaming Service, as provided in the Deezer Streaming Songs User Analytics Competition on Kaggle.

## Objective
The primary objective of this project is to predict whether users of the Deezer app will listen to a given song for at least 30 seconds. This binary classification problem (is_listened = 1 if listened for over 30 seconds, otherwise 0) aims to model user preferences and enhance the listening experience by recommending tracks that align with their tastes.

## Dataset
The dataset originally consists of 7.5 million entries, detailing user interactions with the streaming platform. Due to computational constraints, a 1% random sample of this dataset is utilized for the project. Key features include:

User-specific information (e.g., user_id, user_gender, user_age).
Track-specific details (e.g., genre_id, media_id, album_id).
Contextual information (e.g., context_type indicating the situation in which a song was played).

## Approach
The project employs the Keras Functional API for developing the recommendation models, notable for its flexibility in handling models with complex architectures, non-linear topology, and multiple inputs or outputs. Two primary models are constructed:

***Collaborative Filtering Model:*** This model focuses on learning user and media embeddings to understand and predict user preferences based on historical interactions.
**Hybrid Model:** An advanced version of the first model, it integrates additional contextual information (context_type) to provide a more nuanced understanding of user preferences in different situations.
**Key Features**
Deep Learning: Utilization of neural networks to capture the complex relationships and patterns in user-music interactions.
Keras Functional API: Enabling the creation of sophisticated model architectures beyond simple sequential layers.
Embedding Layers: Learning dense representations of users and media items to capture their latent features.
