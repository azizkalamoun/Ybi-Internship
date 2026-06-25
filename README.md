# Movie Recommendation System

## Overview
This project implements a content-based movie recommendation system using Natural Language Processing (NLP) and machine learning techniques. It suggests movies similar to a user-selected title based on metadata such as genres, keywords, tagline, cast, and director.

## Features
- Content-based filtering using movie metadata
- TF-IDF vectorization of combined textual features
- Cosine similarity computation between movies
- Fuzzy matching for user input using movie title similarity
- Top-N movie recommendations (default: 30 suggestions)

## Technologies Used
- Python
- NumPy
- Pandas
- scikit-learn
- Difflib

## Dataset
The system uses a CSV dataset (`movies.csv`) containing:
- Title
- Genres
- Keywords
- Tagline
- Cast
- Director

## How It Works
1. Load and preprocess the dataset
2. Select relevant features (genres, keywords, tagline, cast, director)
3. Handle missing values by replacing them with empty strings
4. Combine all selected features into a single text field
5. Convert text data into numerical vectors using TF-IDF
6. Compute cosine similarity between all movie vectors
7. Accept user input for a favorite movie
8. Find the closest matching title using fuzzy string matching
9. Recommend movies with highest similarity scores

## Usage
Run the script and enter a movie name when prompted:

```bash
Enter your favourite movie name: Inception
