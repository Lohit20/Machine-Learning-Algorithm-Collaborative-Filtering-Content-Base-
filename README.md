# Machine-Learning-Algorithm-Collaborative-Filtering-Content-Base-

# Overview
  This repository provides code for two recommendation systems: Collaborative Filtering and Content-Based Filtering. The systems aim to provide personalized movie recommendations to users based on their preferences and movie characteristics. The Collaborative Filtering system focuses on user similarity and past ratings, while the Content-Based Filtering system leverages movie attributes such as genre. By combining these approaches, the repository offers a comprehensive recommendation solution.

# Dataset
  The code utilizes the MovieLens dataset, which serves as a benchmark dataset for recommendation systems. The dataset contains a large collection of movie ratings provided by users, along with movie metadata including genre, release year, and tags. These data points form the foundation for training and evaluating the recommendation systems.

# Data Preprocessing
    The data preprocessing steps include loading the movies and ratings datasets using pandas, and performing necessary transformations to prepare the data for the recommendation systems. The code converts the ratings dataset into a pivot table, where rows represent users, columns represent movies, and values represent ratings. Any missing values are handled appropriately, such as filling them with zeros. This preprocessing ensures that the data is in a suitable format for further processing.

# Methodology
  The recommendation systems employ different methodologies to generate movie recommendations:
    
    1. Collaborative Filtering:
        - Collaborative Filtering focuses on identifying similar users based on their movie preferences.
        - It calculates cosine similarity between users to determine their similarity scores.
        - Mean-centered prediction is used to estimate movie ratings for the active user based on their similarity to other users.
       
    3. Content-Based Filtering:
    
        - Content-Based Filtering emphasizes the characteristics of movies, such as genre.
        - User profiles are created based on their past movie ratings and associated movie attributes.
        - Cosine similarity is calculated between the user profiles and movie profiles to identify movies that align with the user's preferences.
        By combining these methodologies, the recommendation systems can provide personalized and diverse movie recommendations to users.

# Implementation
    The implementation code within the repository includes functions and algorithms for Collaborative Filtering and Content-Based Filtering:
    
    1. Collaborative Filtering:
        - The code preprocesses the data, calculates cosine similarity between users, and predicts movie ratings using mean-centered prediction.
        - Users can input their ID and optionally a movie ID to receive personalized movie recommendations or an estimated rating for a specific movie.
    
    2. Content-Based Filtering:
        - The code generates user profiles based on past movie ratings and identifies movie recommendations based on cosine similarity between user profiles and movie profiles.
        - Users can input their ID to receive recommendations for the top 3 movies.
        - The code is designed to work with the MovieLens dataset and provides a foundation for building and experimenting with recommendation systems.

# Conclusion

In conclusion, this repository provides code for two recommendation systems: Collaborative Filtering and Content-Based Filtering. These systems aim to offer personalized movie recommendations to users based on their preferences and movie characteristics. By combining user similarity and past ratings in Collaborative Filtering, and leveraging movie attributes such as genre in Content-Based Filtering, the systems provide comprehensive and diverse recommendations.

Overall, the recommendation systems implemented in this repository provide valuable insights into the collaborative and content-based approaches to movie recommendations. They offer a starting point for developing more sophisticated recommendation systems and can contribute to improving user satisfaction and engagement in various movie-related applications.
