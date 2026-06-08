# Recommendation System

A collection of notebook-based recommendation system experiments implemented in Python. This project explores three common recommendation approaches:

1. **Item similarity recommendation for movies** using user rating correlations.
2. **Product recommendation with KNN** using review-based features.
3. **Collaborative filtering for products** using user–item interactions and matrix-based methods.

The repository is organized as a learning project rather than a production-ready package, and most of the work is implemented inside Jupyter notebooks.

## Project Overview

This repository demonstrates multiple ways to build recommender systems with Python, pandas, and scikit-learn. The included notebooks walk through data loading, exploratory analysis, user–item matrix creation, similarity computation, and collaborative filtering workflows.

### Implemented Sections

#### 1) Movie Recommendation with Python
Notebook: `Recommender Systems with Python.ipynb`

This notebook builds a simple **item-based recommendation system** using movie ratings. It:
- loads the MovieLens-style ratings data from `u.data`
- joins movie IDs with movie titles from `Movie_Id_Titles`
- performs exploratory data analysis on ratings
- builds a user–movie rating matrix
- computes correlations between movie rating vectors
- recommends movies similar to a selected title

#### 2) Product Recommendation with KNN
Notebook: `Product Recommender System.ipynb`

This notebook focuses on **product recommendation / review-based modeling**. Based on the notebook contents, it includes:
- filtering products with sufficient review volume
- grouping and summarizing product reviews
- text cleaning for review summaries
- feature extraction from review text
- KNN-based recommendation / similarity workflow
- prediction and evaluation steps for review score modeling

> Note: this notebook references external files such as `reviewsWithHeader.csv` and `ProductReviewSummary.csv`, which are **not included** in the provided ZIP archive.

#### 3) Collaborative Filtering Recommender Model
Notebook: `Collaborative Filtering recommender model.ipynb`

This notebook demonstrates **collaborative filtering** techniques using user behavior data. Based on the notebook structure, it covers:
- loading product ratings data
- cleaning and subsetting a large ratings dataset
- handling sparsity by selecting active users / frequently rated items
- building a user–item matrix
- similarity computation with cosine similarity / nearest neighbors
- sparse matrix operations
- matrix factorization concepts such as SVD

> Note: this notebook references `ratings_Electronics.csv`, which is **not included** in the provided ZIP archive.

## Repository Structure

```text
Recommendation-System-master/
├── Collaborative Filtering recommender model.ipynb
├── Product Recommender System.ipynb
├── Recommender Systems with Python.ipynb
└── u.data
