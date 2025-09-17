# Book-Recommender-System

📚 Book Recommendation System

A Book Recommendation System using Collaborative Filtering and Content-Based Filtering. Built with Python, Pandas, Scikit-Learn, NLTK, and Gensim.

Features

Collaborative Filtering with cosine similarity and Nearest Neighbors

Content-Based Filtering using Word2Vec embeddings

Exploratory Data Analysis: top authors, books, publishers, and active users

Filtering for experienced users and popular books

Dataset

Books.csv → book details

Ratings.csv → user ratings

Users.csv → user demographics

Extract the dataset before running:

!unzip "Machine Learning-20250914T055612Z-1-001.zip"

Installation
pip install numpy pandas matplotlib seaborn scikit-learn nltk gensim tensorflow joblib


NLTK downloads:

import nltk
nltk.download('punkt')

Usage
Collaborative Filtering
recommend("1984")          # top similar books
recommend_nn("River's End") # KNN-based recommendation

Content-Based Filtering
recommend_books("Echoes", k=5)  # content similarity-based recommendation

Insights

Most books published: 2002

Top publisher: Harlequin

Most active user: ID 11676

Most rated book: Wild Animus

Tech Stack

Python, Pandas, Numpy, Scikit-Learn, NLTK, Gensim, TensorFlow, Matplotlib, Seaborn
