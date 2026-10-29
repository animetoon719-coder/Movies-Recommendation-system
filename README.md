# Movie Recommendation System

## 1. Project Overview

The Movie Recommendation System is a machine learning project that recommends movies similar to a movie selected by the user.

The system analyzes movie genres and uses text processing and similarity measurement techniques to identify movies with similar characteristics.

For example, if a user selects *Toy Story (1995)*, the system recommends other movies belonging to similar genres, such as animation, adventure, comedy, and children's movies.

The project is developed using Python and Google Colab. It uses the MovieLens dataset for movie information and ratings.

## 2. Problem Statement

With a large number of movies available, users may find it difficult to choose what to watch next.

This project aims to solve this problem by developing a simple recommendation system that suggests movies based on genre similarity.

## 3. Project Objectives

* To develop a basic movie recommendation system using Python.
* To process and analyze movie dataset information.
* To identify similar movies using their genres.
* To apply TF-IDF vectorization and cosine similarity.
* To recommend the top 10 similar movies for a selected movie.
* To understand the practical application of machine learning and data processing techniques.

## 4. Technologies Used

* **Python:** Main programming language.
* **Google Colab:** Cloud-based coding and execution environment.
* **Pandas:** Data loading, cleaning, and manipulation.
* **Scikit-learn:** Machine learning and text-processing utilities.
* **TF-IDF Vectorization:** Converts movie genre text into numerical features.
* **Cosine Similarity:** Measures similarity between movie feature vectors.
* **Jupyter Notebook:** Interactive environment for code and results.
* **GitHub:** Project code hosting and version control.

## 5. Dataset Description

The project uses two CSV files from the MovieLens movie-rating dataset.

### Movie Dataset — movie.csv

The movie dataset contains information about movies.

| Column  | Description                      |
| ------- | -------------------------------- |
| movieId | Unique identifier of a movie     |
| title   | Movie title and release year     |
| genres  | Genres associated with the movie |

### Rating Dataset — rating.csv

The rating dataset contains user ratings for movies.

| Column    | Description                       |
| --------- | --------------------------------- |
| userId    | Identifier of the user            |
| movieId   | Identifier of the rated movie     |
| rating    | Rating given by the user          |
| timestamp | Time when the rating was recorded |

The current genre-based recommendation method primarily uses the movie title and genres. The rating dataset is available for possible future improvements, such as collaborative filtering.

## 6. Methodology

The system follows these steps:

1. Load the movie and rating CSV files into Google Colab.
2. Inspect the dataset columns and understand the data.
3. Select the movie information required for recommendations.
4. Convert genre text into numerical features using TF-IDF vectorization.
5. Calculate cosine similarity between movie feature vectors.
6. Select the movie entered by the user.
7. Rank other movies according to their similarity.
8. Display the top 10 recommended movies with their genres and similarity scores.

## 7. Algorithm Used

### TF-IDF Vectorization

TF-IDF stands for Term Frequency–Inverse Document Frequency. It is a technique used to convert text into numerical features.

In this project, movie genres are treated as text. TF-IDF converts the genre information into vectors that can be compared mathematically.

### Cosine Similarity

Cosine similarity measures how similar two numerical vectors are.

The formula is:

Cosine Similarity = (A · B) / (||A|| × ||B||)

Here, A and B represent the feature vectors of two movies.

A higher similarity score indicates that the movies have more similar genre representations.

## 8. Example Output

**Selected Movie:** Toy Story (1995)

Example recommended movies include:

* Antz (1998)
* Toy Story 2 (1999)
* Monsters, Inc. (2001)
* The Emperor's New Groove (2000)

These movies share similar genre information with the selected movie.

The exact recommendations and similarity scores depend on the dataset and implementation.

## 9. How to Run the Project

1. Open the project Jupyter Notebook file from this repository.
2. Open it in Google Colab.
3. Upload `movie.csv` and `rating.csv` when required by the notebook.
4. Run the notebook cells in the correct order.
5. Select a movie supported by the dataset.
6. View the recommended movies in the output.

## 10. Applications

* Movie discovery and entertainment platforms.
* Personalized content recommendation.
* Exploring movie genres and similarities.
* Learning basic recommendation algorithms.
* Understanding text vectorization and similarity measurement.

## 11. Advantages

* Simple and beginner-friendly implementation.
* Provides recommendations based on movie genres.
* Uses widely available Python libraries.
* Can process a large collection of movie records.
* Demonstrates a practical application of data science concepts.

## 12. Limitations

* Recommendations depend heavily on the available genre information.
* Movies with identical genre representations may receive the same similarity score.
* The current genre-based method does not necessarily personalize results for individual users.
* The rating dataset is not the primary input to the current genre-based recommendation calculation.
* Recommendation quality depends on the completeness and quality of the dataset.

## 13. Future Scope

* Implement collaborative filtering using user ratings.
* Develop a hybrid recommendation system combining genres and ratings.
* Build an interactive web interface using Streamlit.
* Add movie posters, descriptions, and release information.
* Allow users to select movies through a search box.
* Evaluate recommendation quality using suitable recommendation metrics.

## 14. Conclusion

The Movie Recommendation System demonstrates how Python, data processing, text vectorization, and cosine similarity can be combined to recommend similar movies.

The project provides practical experience with datasets, machine learning tools, and recommendation algorithms. It can be extended into a more personalized system by incorporating user ratings and additional movie information.

## 15. References

* MovieLens: https://grouplens.org/datasets/movielens/
* Pandas Documentation: https://pandas.pydata.org/docs/
* Scikit-learn Documentation: https://scikit-learn.org/stable/
* Google Colab: https://colab.research.google.com/

## Project Repository

This repository contains the Jupyter Notebook used to implement the Movie Recommendation System.

**Note:** The implementation and output should be verified by running the notebook in Google Colab.

