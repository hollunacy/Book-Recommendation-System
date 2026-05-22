# Book Recommendation System
A Python-based hybrid recommendation system built on the Goodreads dataset. The project implements multiple recommendation strategies to improve prediction accuracy and mitigate the cold-start problem.

## Key Features & Methodology
- **Data Preprocessing & Cleaning:** Processed semi-structured JSON arrays, eliminated linguistic noise, and handled implicit interactions (zero/missing ratings).
- **NLP Pipeline (NLTK):** Implemented text tokenization, normalization, stop-word removal, and TF-IDF vectorization for content-based profile building.
- **Model Development:** 
  - Built Content-Based filtering using Cosine Similarity.
  - Implemented Collaborative Filtering models (Item-based KNN, SVD).
  - Designed Weighted and Switching hybrid strategies.
- **Evaluation & Optimization:** Conducted offline validation on 140,000+ test records using accuracy metrics (MAE, RMSE) and ranking metrics (Precision@K, Recall@K, F1-score).

## Tech Stack
- **Language:** Python
- **Libraries:** Pandas, NumPy, Scikit-learn, Surprise, NLTK
- **Data Format:** JSON, CSV

## Data Source
The dataset used in this project is the official UCSD Goodreads dataset, which contains book metadata, reviews, and user interactions collected for academic research: [Goodreads Book Graph Datasets]([https://ucsd.edu](https://cseweb.ucsd.edu/~jmcauley/datasets/goodreads.html))
