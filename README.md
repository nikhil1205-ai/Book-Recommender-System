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

```bash
!unzip "/content/Machine Learning-20250914T055612Z-1-001.zip"

