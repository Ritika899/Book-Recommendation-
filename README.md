# 📚 Book Recommendation System

## 📌 Overview

This project builds a **Book Recommendation System** using the Book-Crossing dataset. It provides recommendations using two approaches:

* ⭐ **Popularity-Based Recommendation**
* 👥 **Collaborative Filtering**

The collaborative filtering model uses **Cosine Similarity** to identify books similar to a selected book based on user ratings.

## 📂 Dataset

The dataset contains three files:

* `Books.csv` – Book details such as title, author, publisher and ISBN
* `Ratings.csv` – User ratings for books
* `Users.csv` – User information such as location and age

### 🔗 Kaggle Dataset

The dataset can be downloaded directly from Kaggle:

**[Book Recommendation Dataset – Kaggle](https://www.kaggle.com/datasets/arashnic/book-recommendation-dataset)**

## 🛠️ Tools & Libraries

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

## 🔍 Methodology

### 1. Data Preprocessing

* Loaded the three datasets.
* Checked data types, missing values and duplicates.
* Merged books and ratings using `ISBN`.

### 2. Popularity-Based Recommendation

Books are ranked based on:

* Number of ratings
* Average rating

Books with at least **250 ratings** are considered and sorted according to their average rating.

### 3. Collaborative Filtering

* Selected users with more than **200 ratings**.
* Selected books with at least **50 ratings**.
* Created a user-book rating matrix.
* Calculated **Cosine Similarity** between books.
* Generated recommendations for a given book.

Example:

```python
suggest('Animal Farm')
```

## 📊 Output

The system returns a list of similar/recommended books along with:

* 📖 Book Title
* ✍️ Author
* 🖼️ Book Cover Image

## 📁 Repository Structure

```text
Book-Recommendation-System/
│
├── book recommendation (1).ipynb
├── Books.csv
├── Ratings.csv
├── Users.csv
└── README.md
```
