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
| pandas | latest | Data loading and manipulation |
| scikit-learn | latest | `NearestNeighbors` kNN implementation |

---

## Dataset

**File:** `movies_recommendation_data.csv`  
**Source:** [https://github.com/ArinB/MSBA-CA-Data/raw/main/CA05/movies_recommendation_data.csv](https://github.com/ArinB/MSBA-CA-Data/raw/main/CA05/movies_recommendation_data.csv)

The dataset contains 30 movies, each described by 8 numerical features:

| Feature | Type | Description |
|---|---|---|
| IMDB Rating | Continuous | Movie rating on IMDB (range ~5.9–8.8) |
| Biography | Binary (0/1) | Whether the movie is a biographical film |
| Drama | Binary (0/1) | Whether the movie is a drama |
| Thriller | Binary (0/1) | Whether the movie is a thriller |
| Comedy | Binary (0/1) | Whether the movie is a comedy |
| Crime | Binary (0/1) | Whether the movie involves crime |
| Mystery | Binary (0/1) | Whether the movie is a mystery |
| History | Binary (0/1) | Whether the movie is historical |

> The `Label` column (all zeros) and identifier columns (`Movie ID`, `Movie Name`) are dropped before modeling.

The dataset is loaded directly from the URL in the notebook — no manual download needed.

---

## How to Install and Run

### 1. Clone the repository

### 2. Install required libraries

### 3. Run the notebook

The dataset is fetched automatically from GitHub inside the notebook — no additional setup needed.

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

- Dataset accessed via course materials provided by Professor Arin Brahma, Loyola Marymount University: [https://github.com/ArinB/MSBA-CA-Data](https://github.com/ArinB/MSBA-CA-Data).
