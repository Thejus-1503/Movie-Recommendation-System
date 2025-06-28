# Movie-Recommendation-System

# 🎬 Movie Recommendation System (Matrix Factorization from Scratch)

This project is a **movie recommendation system** built entirely from scratch using **NumPy** and classic **matrix factorization** techniques. It was developed as part of my learning journey in recommendation systems and collaborative filtering, without relying on external libraries like Surprise or LightFM.

---

## 🧠 Objective

To implement a fully interpretable and modular movie recommendation engine using:
- Matrix factorization via gradient descent
- Genre-based and popularity-based filtering
- Collaborative filtering using user–movie interaction data

---

## 🔧 Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib (for visualizations)

No machine learning libraries (like `Surprise` or `scikit-learn`) were used for modeling.

---

## 🚀 Features

### 1. **Matrix Factorization**
- Built from scratch using gradient descent
- Learned latent **user** and **item** features
- Predicted unseen movie ratings by reconstructing the rating matrix

### 2. **Top-N Recommendations**
- Recommended top-rated movies based on average user ratings

### 3. **Most Popular by Year**
- Identified frequently rated movies per year to capture popularity trends

### 4. **Genre-Based Filtering**
- Allowed filtering recommendations based on user-preferred genres

---

## 📈 How It Works

1. **Data Preprocessing**
   - Merged `ratings.csv` and `movies.csv`
   - Created a user–movie rating matrix via pivot tables

2. **Matrix Factorization**
   - Used gradient descent to decompose the matrix into two lower-dimensional matrices
   - Optimized to minimize the mean squared error for known ratings

3. **Prediction**
   - Reconstructed full rating matrix to estimate missing ratings

4. **Recommendation Logic**
   - Personalized results using hybrid strategies (collaborative + content-based)
