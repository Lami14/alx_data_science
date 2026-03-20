# 🧠 Unsupervised Machine Learning Portfolio

A collection of unsupervised machine learning projects built with Python and Scikit-learn, exploring clustering, dimensionality reduction, probabilistic modelling, and recommendation systems on real-world datasets.

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.x-F7931E?logo=scikitlearn)
![Pandas](https://img.shields.io/badge/Pandas-2.x-150458?logo=pandas)
![GeoPandas](https://img.shields.io/badge/GeoPandas-0.14-4CAF50)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.x-11557c)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

---

## 📁 Projects Overview

| Folder | Technique | Description |
|---|---|---|
| `kmean-hierarchical_clustering` | K-Means + Hierarchical | Segment data into meaningful groups |
| `gaussian_mixture` | Gaussian Mixture Models | Probabilistic soft-assignment clustering |
| `principal_component_analysis` | PCA | Reduce high-dimensional data while preserving variance |
| `dimensional_reduction` | t-SNE / UMAP | Non-linear dimensionality reduction for visualisation |
| `recommendation_system` | Collaborative Filtering | Build a personalised item recommendation engine |
| `clustering_geospatial` | K-Means + GeoPandas | Cluster world countries by GDP and population on a map |

---

## 🗂️ Project Details

### 1. 📍 Clustering & Geospatial Analysis
Applied K-Means clustering on world country data using GDP and population as features, then visualised the results as choropleth maps and multidimensional scatter overlays.

**Key techniques:**
- K-Means clustering on economic indicators
- Geospatial visualisation with GeoPandas
- Multidimensional plotting — colour (GDP), size (population), shape (continent)
- Coordinate Reference System (CRS) handling

**Dataset:** Natural Earth Low Resolution — country geometries, GDP, population, continent

---

### 2. 📊 K-Means & Hierarchical Clustering
Compared flat (K-Means) and hierarchical (agglomerative) clustering approaches on structured datasets. Used the elbow method to determine optimal cluster count and dendrograms to visualise merge distances.

**Key techniques:**
- K-Means with elbow method for optimal k
- Agglomerative hierarchical clustering
- Dendrogram visualisation
- Silhouette score evaluation

---

### 3. 🌊 Gaussian Mixture Models
Modelled data distributions using probabilistic Gaussian Mixture Models (GMM), allowing soft cluster assignments where each data point has a probability of belonging to each cluster.

**Key techniques:**
- Expectation-Maximisation (EM) algorithm
- Soft vs hard cluster assignment
- BIC/AIC model selection
- Comparison with K-Means hard clustering

---

### 4. 📉 Principal Component Analysis (PCA)
Applied PCA to reduce high-dimensional datasets to 2–3 components while retaining maximum variance, enabling faster modelling and cleaner visualisations.

**Key techniques:**
- Explained variance ratio analysis
- Scree plots for component selection
- 2D and 3D PCA projections
- PCA as preprocessing for downstream ML

---

### 5. 🔍 Dimensionality Reduction (t-SNE / UMAP)
Used non-linear dimensionality reduction techniques to reveal hidden structure in high-dimensional data that PCA cannot capture linearly.

**Key techniques:**
- t-SNE for cluster visualisation
- UMAP for faster non-linear projection
- Comparison of linear vs non-linear reduction
- Hyperparameter tuning (perplexity, n_neighbors)

---

### 6. 🎯 Recommendation System
Built a collaborative filtering recommendation engine that suggests items to users based on patterns in historical interactions — the same approach used by Netflix and Spotify.

**Key techniques:**
- User-based and item-based collaborative filtering
- Cosine similarity for user/item matching
- Matrix factorisation concepts
- Evaluation with precision and recall

---

## 🛠️ Tech Stack

| Library | Purpose |
|---|---|
| `scikit-learn` | Clustering, PCA, GMM, model evaluation |
| `pandas` | Data loading, manipulation |
| `numpy` | Numerical computation |
| `matplotlib` | All visualisations and plots |
| `seaborn` | Statistical visualisation |
| `geopandas` | Geospatial data handling and mapping |
| `shapely` | Geometric operations |

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/Lami14/alx_data_science.git
cd alx_data_science
```

### 2. Install dependencies
```bash
pip install scikit-learn pandas numpy matplotlib seaborn geopandas shapely
```

### 3. Open any project
```bash
cd kmean-hierarchical_clustering
jupyter notebook
```

> Each folder contains its own notebook with inline explanations and outputs.

---

## 💡 What I Learned

- How unsupervised learning finds hidden structure in unlabelled data
- When to choose K-Means vs GMM vs hierarchical clustering for a given problem
- How PCA and t-SNE complement each other — PCA for speed, t-SNE for visualisation
- How real-world recommendation systems work under the hood using similarity metrics
- How to represent economic and demographic data visually on geographic maps

---

## 🔮 Future Improvements

- [ ] Add evaluation metrics (silhouette score, Davies-Bouldin index) across all projects
- [ ] Deploy the recommendation system as a Flask API
- [ ] Add an interactive map dashboard using Folium or Plotly
- [ ] Extend geospatial analysis with South African provincial data

---

## 📄 License

MIT License — feel free to fork and build on this work.

---

*Built by [Lamla](https://github.com/Lami14) · Unsupervised ML Portfolio · ALX Africa Data Science Programme 🇿🇦*
