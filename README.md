# Movie Recommendation System

A content-based movie recommendation system built using Python, pandas, scikit-learn, NLTK, and Streamlit.

## Overview
This project recommends similar movies based on movie metadata such as genres, keywords, cast, and crew. It uses feature engineering and cosine similarity to build a recommendation engine.

## Features
- Content-based movie recommendations
- Cosine similarity for finding similar movies
- Streamlit web app interface
- Data preprocessing and feature engineering
- TMDB 5000 movie dataset

## Tech Stack
- Python
- pandas
- scikit-learn
- NLTK
- Streamlit

## Dataset
This project uses the TMDB 5000 Movies Dataset:
- `tmdb_5000_movies.csv`
- `tmdb_5000_credits.csv`

## Project Structure
```bash
movie-recommendation-system/
│
├── app/
│   └── app.py
├── notebooks/
│   └── movie_recommender_analysis.ipynb
├── src/
│   ├── data_preprocessing.py
│   ├── feature_engineering.py
│   └── recommender.py
├── .gitignore
├── README.md
├── movies_dict.pkl
├── requirements.txt
├── tmdb_5000_credits.csv
└── tmdb_5000_movies.csv
```

## How It Works
1. Load and merge movie and credits datasets
2. Preprocess important columns
3. Perform feature engineering on metadata
4. Convert text features into vectors
5. Compute cosine similarity between movies
6. Recommend the most similar movies

## Installation
Clone the repository:

```bash
git clone https://github.com/tanviparmar0317-oss/movie-recommendation-system.git
cd movie-recommendation-system
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Run the App

```bash
streamlit run app/app.py
```

## Note
The large `similarity.pkl` file is not included in this repository because of GitHub file size limits. You can regenerate it by running the preprocessing and recommendation pipeline.

## Author
Tanvi Parmar
