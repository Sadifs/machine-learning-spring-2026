# CA05 – kNN Based Movie Recommender Engine

## Description
This project builds a content-based movie recommendation engine using the **k-Nearest Neighbors (kNN)** algorithm. Given a query movie, the engine searches a dataset of 30 films and returns the 5 most similar movies based on genre attributes and IMDB rating.

**Core question:** *What are the 5 movies most similar to "The Post"?*

A user browsing a movie website encounters *The Post* and wants to see similar titles. The engine takes the movie's feature vector (genres + rating), computes Euclidean distances across all movies in the dataset, and returns the top 5 nearest neighbors.

---

## Libraries & Versions

| Library | Version | Purpose |
|---|---|---|
| Python | 3.13.5 | Runtime environment |
| pandas | 2.2.3 | Data loading and manipulation |
| scikit-learn | 1.6.1 | `NearestNeighbors` kNN implementation |

---

## Dataset

**File:** `movies_recommendation_data.csv`  
**Source:** https://github.com/ArinB/MSBA-CA-Data/raw/main/CA05/movies_recommendation_data.csv

The dataset contains 30 movies, each described by 8 numerical features: IMDB Rating, Biography, Drama, Thriller, Comedy, Crime, Mystery, and History. The `Label` column and identifier columns (`Movie ID`, `Movie Name`) are dropped before modeling. The dataset loads automatically from the URL — no manual download needed.

---

## How to Install and Run

### 1. Install required libraries
```bash
pip install pandas scikit-learn
```

### 2. Run the notebook
Open `CA05_kNN_Recommender.ipynb` in Jupyter and run all cells top to bottom:
```bash
jupyter notebook CA05_kNN_Recommender.ipynb
```

---

## Results

The 5 most similar movies to *The Post* (IMDB: 7.2 | Biography, Drama, History), ranked by Euclidean distance:

| Rank | Movie | IMDB Rating | Distance |
|---|---|---|---|
| 1 | 12 Years a Slave | 8.1 | 0.900 |
| 2 | Hacksaw Ridge | 8.2 | 1.000 |
| 3 | Queen of Katwe | 7.4 | 1.020 |
| 4 | The Wind Rises | 7.8 | 1.166 |
| 5 | A Beautiful Mind | 8.2 | 1.414 |

---

## Acknowledgements

Dataset sourced from the UCI Machine Learning Repository IMDB dataset, accessed via course materials provided by Professor Arin Brahma, Loyola Marymount University. Original repository: https://github.com/ArinB/MSBA-CA-Data
