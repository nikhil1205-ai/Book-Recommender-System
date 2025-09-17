# Book-Recommender-System

# 📚 Book Recommendation System

This project builds a **Book Recommendation System** using both **Collaborative Filtering** and **Content-Based Filtering** approaches.  
It uses the popular **Books, Ratings, and Users dataset** from Kaggle.

---

## 🚀 Features

- **Data Cleaning & Preprocessing**:  
  Handle missing values, duplicates, and inconsistent data.

- **Exploratory Data Analysis (EDA)**:  
  - Top years with most publications  
  - Most active publishers  
  - Distribution of ratings  
  - Most active users  
  - Most rated books and top authors

- **Collaborative Filtering**:  
  - User–Book rating matrix  
  - Cosine similarity between books  
  - Nearest Neighbors model  
  - Clustering with KMeans and Gaussian Mixture

- **Content-Based Filtering**:  
  - Text preprocessing of book title, author, and publisher  
  - Word2Vec embeddings for semantic similarity  
  - Cosine similarity to recommend books based on content

---

## 📂 Dataset

The dataset contains three files:

- **Books.csv** → Information about books (Title, Author, Publisher, Year, Images)  
- **Ratings.csv** → User ratings for books  
- **Users.csv** → User demographic details

⚠️ You need to unzip the dataset before running:



## 🛠️ Installation

- Install dependencies (if not already installed):
- pip install numpy pandas matplotlib seaborn scikit-learn nltk gensim tensorflow joblib


## Download NLTK resources:

- import nltk
- nltk.download('punkt')

## 📊 Workflow
- 1. Data Cleaning

Fill missing authors, publishers, and image URLs.

Remove duplicates.

2. Exploratory Data Analysis (EDA)

Top years, publishers, authors, most rated books, and most active users.

3. Collaborative Filtering

Filter active users (>200 ratings)

Filter popular books (≥50 ratings)

Create book–user pivot matrix

Apply:

Cosine similarity

KNN (Nearest Neighbors)

Clustering (KMeans, Gaussian Mixture)

4. Content-Based Filtering

Combine Title + Author + Publisher into single text

Preprocess text (lowercase, remove special chars, tokenize)

Train Word2Vec to create embeddings

Compute cosine similarity between book vectors

## 🔎 Example Usage
Collaborative Filtering
recommend("1984")
Returns similar books to 1984.

recommend_nn("River's End")


Returns recommendations using Nearest Neighbors.

Content-Based Filtering
recommend_books("Echoes", k=5)


Returns 5 similar books to Echoes based on content similarity.

## 📌 Key Insights

2002 had the most books published.

Harlequin was the top publisher.

Over 50% of ratings are zero, so filtering active users is important.

William Shakespeare has the most books in the dataset.

Wild Animus is the most rated book.

User with ID 11676 gave the most ratings (11,144).

## 🧑‍💻 Tech Stack

Python 3

Pandas, Numpy → Data processing

Matplotlib, Seaborn → Visualization

Scikit-Learn → ML models & similarity

NLTK, Gensim → Text processing, Word2Vec

TensorFlow / Keras → DL support
