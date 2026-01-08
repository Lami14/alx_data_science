

📊 Gaussian Mixture Models (GMM) – Clustering Analysis

Advanced Unsupervised Learning Project
© ExploreAI Academy

This project explores Gaussian Mixture Models (GMMs) applied to the Iris dataset, focusing on clustering behavior, model selection using Bayesian Information Criterion (BIC), and the impact of different covariance types. Dimensionality reduction using PCA is employed for visualization and interpretability.


---

🚀 Project Objectives

By completing this project, I demonstrated the ability to:

Implement Gaussian Mixture Models using Scikit-learn

Apply PCA for dimensionality reduction and visualization

Determine the optimal number of clusters using BIC

Analyze the effect of different covariance types

Interpret clustering outcomes and patterns in real datasets



---

📂 Dataset Overview

Iris Dataset

Introduced by Sir Ronald Fisher (1936)

150 samples, 3 species

4 numerical features:

Sepal length

Sepal width

Petal length

Petal width



Target species:

Iris Setosa

Iris Versicolor

Iris Virginica



---

🛠️ Technologies & Libraries

Python 3

NumPy

Pandas

Scikit-learn

Matplotlib



---

📘 Project Workflow


---

1️⃣ Data Loading & Exploration

Loaded the Iris dataset using load_iris()

Converted features into a Pandas DataFrame

Verified data quality (no missing values)



---

2️⃣ Dimensionality Reduction with PCA

Reduced feature space from 4D → 2D

Enabled clear visualization of natural groupings

PCA revealed strong separation of Setosa, with partial overlap between Versicolor and Virginica


📌 Insight: PCA preserves global structure while simplifying visualization.


---

3️⃣ Gaussian Mixture Model (Basic Application)

Applied GMM with 3 components (based on known species)

Fitted the model to PCA-reduced data

Predicted cluster assignments


📌 Observation:
GMM successfully captured cluster structure, especially for Setosa, while overlapping species showed softer boundaries—consistent with real data distributions.


---

4️⃣ Optimal Cluster Selection using BIC

Evaluated GMMs with 1–6 components

Used Bayesian Information Criterion (BIC) for model comparison

Lower BIC indicates a better balance between model fit and complexity


📉 Result:
The BIC curve suggested 2 clusters as optimal, highlighting that unsupervised learning may differ from labeled ground truth.

📌 Key takeaway:
Optimal statistical clustering does not always match human-defined classes.


---

5️⃣ Effect of Covariance Types

Tested four covariance structures:

Covariance Type	Interpretation

full	Most flexible, captures full feature relationships
tied	Shared covariance across clusters
diag	Independent features
spherical	Equal variance in all directions


📌 Findings:

full covariance provided the most expressive clustering

spherical produced the simplest but least accurate clusters

Covariance choice significantly impacts cluster shape and separation



---

📈 Visual Outputs

PCA-reduced scatter plot colored by species

GMM clustering visualizations

BIC score vs number of components

Cluster plots for each covariance type



---

🧠 Key Learnings

GMMs are probabilistic and more flexible than K-Means

BIC is a powerful tool for model selection

Covariance structure directly affects cluster geometry

Dimensionality reduction improves interpretability but may affect cluster boundaries

