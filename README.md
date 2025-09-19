# Movie-Recommendator
A Movie Recommendation System built using collaborative filtering with a focus on item-based collaborative filtering. This project leverages the Kaggle movie dataset to provide personalized movie recommendations by analyzing user-item interactions and similarities.

🚀 Features

Collaborative Filtering: Finds recommendations by analyzing relationships between users and movies.

Item-Based Filtering: Suggests movies similar to a given movie using similarity scores.

Similarity Computation: Uses k-Nearest Neighbors (KNN) and RapidFuzz for efficient similarity matching.

Clean & Scalable Pipeline: Built with pandas and NumPy for preprocessing and matrix manipulation.

Machine Learning Integration: Powered by scikit-learn for model building and evaluation.

🛠️ Tech Stack

Python 🐍

Pandas → Data manipulation & preprocessing

NumPy → Matrix operations

scikit-learn → Machine learning (KNN implementation)

RapidFuzz → Fuzzy string matching for movie titles

Kaggle Dataset → Source of movie ratings and metadata

📊 How It Works

Load and preprocess the dataset (movies, users, and ratings).

Build a user-item interaction matrix.

Apply item-based collaborative filtering using cosine similarity / KNN.

Use RapidFuzz for approximate movie title matching.

Generate top-N recommendations for a selected movie.

📂 Dataset

Dataset taken from Kaggle

Includes movie metadata and user ratings.

🎯 Example Usage
# Example: Get top 10 recommendations for a movie
recommendations = recommendor("The Matrix", user_item_matrix, knn_model, 10, movie_data)
print(recommendations)

📌 Future Improvements

Add user-based collaborative filtering

Hybrid approach combining content + collaborative filtering

Web UI for interactive recommendations
