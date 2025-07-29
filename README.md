# 🎬 Movie Recommendation System

This project builds a **content-based movie recommendation system** using metadata from movies such as title, genre, cast, crew, and overview. It aims to suggest similar movies to users based on the content of movies they like.

## 📁 Project Structure

```
Movie-Recommendation-System/
├── Movie Recommendation.ipynb       # Main notebook with all code and analysis
├── movies_metadata.csv              # Dataset with movie metadata
├── movies_metadata.zip              # Compressed dataset
└── README.md                        # Project documentation
```

## 📌 Features

- ✅ Load and clean metadata from the TMDB 5000 movie dataset  
- ✅ Parse genres, keywords, cast, crew, and overview  
- ✅ Text preprocessing using TF-IDF and CountVectorizer  
- ✅ Content-based recommendations using cosine similarity  
- ✅ Function to recommend top 10 similar movies  
- ✅ Visualizations and movie metadata exploration  

## 🧠 Technologies Used

- Python 3
- Jupyter Notebook
- Pandas
- NumPy
- Scikit-learn
- NLTK (optional for text cleaning)
- Matplotlib / Seaborn (for optional visualizations)



## 📊 Dataset


- **File**: `movies_metadata.csv`
- Contains over 45,000 movie records with attributes such as:
  - Title
  - Genres
  - Overview
  - Cast & Crew
  - Keywords
  - Popularity, Revenue, Vote Average, etc.

## 🧪 How It Works

- Extract important metadata from the dataset
- Convert text features (overview, genres, keywords, etc.) into numeric vectors
- Calculate **cosine similarity** between vectors
- Recommend movies with the most similar vectors to the input movie

## 🔍 Example

```python
get_recommendations('The Dark Knight')
```

This returns a list of 10 movies that are similar in content and themes to *The Dark Knight*.

## 📌 Future Improvements

- Add collaborative filtering with user ratings
- Hybrid recommendations (Content + Collaborative)
- Deploy as a Flask web app
- Integrate with live TMDB API for real-time data
