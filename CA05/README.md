# CA05 – kNN Based Movie Recommender Engine

## Description
This project builds a movie recommendation engine using the k-Nearest Neighbors (kNN) algorithm. Given a query movie ("The Post"), it identifies the 5 most similar movies from a 30-movie dataset based on genre attributes and IMDB rating.

## Libraries & Versions
- Python 3.13.5
- pandas
- scikit-learn

## Dataset
**File:** `movies_recommendation_data.csv`  
**Source:** https://github.com/ArinB/MSBA-CA-Data/raw/main/CA05/movies_recommendation_data.csv  
30 movies with 8 features: IMDB Rating, Biography, Drama, Thriller, Comedy, Crime, Mystery, History.

## How to Install and Run
1. Install dependencies:
```bash
pip install pandas scikit-learn
```
2. Open and run all cells in `CA05_kNN_Recommender.ipynb`. The dataset loads automatically from the URL.

## Acknowledgements
Dataset sourced from the UCI Machine Learning Repository IMDB dataset, provided via course materials by Professor Arin Brahma, LMU. Original repo: https://github.com/ArinB/MSBA-CA-Data
