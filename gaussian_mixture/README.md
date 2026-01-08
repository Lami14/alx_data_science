Gaussian Mixture Models (GMM) – Iris Dataset
Exercise: Gaussian Mixture Models
© ExploreAI Academy
This project applies Gaussian Mixture Models (GMMs) to the classic Iris dataset to explore clustering behavior, determine the optimal number of clusters using Bayesian Information Criterion (BIC), and analyze the impact of different covariance structures on clustering results.
🎯 Learning Objectives
By completing this exercise, you will be able to:
Implement Gaussian Mixture Models using Scikit-learn
Apply PCA for dimensionality reduction prior to clustering
Evaluate clustering performance using BIC
Understand how covariance types affect clustering outcomes
📂 Dataset
Iris Dataset (Fisher, 1936)
150 samples
4 numerical features:
Sepal length
Sepal width
Petal length
Petal width
3 species:
Iris setosa
Iris versicolor
Iris virginica
Loaded using:
Copy code
Python
from sklearn.datasets import load_iris
🛠️ Technologies Used
Python 🐍
Scikit-learn
Pandas
NumPy
Matplotlib
📘 Exercises Overview
Exercise 1: Data Loading & PCA
Loaded the Iris dataset
Applied PCA to reduce dimensionality from 4D → 2D
Visualized natural clusters using true species labels
Observation:
Setosa is clearly separated
Versicolor and Virginica show partial overlap
Exercise 2: Basic GMM Application
Applied Gaussian Mixture Model with:
n_components = 3
Fitted model on PCA-reduced data
Visualized clusters in 2D space
Observation:
GMM effectively captures elliptical cluster structures
Results align reasonably well with actual species labels
Exercise 3: Optimal Number of Clusters (BIC)
Trained GMMs with 1–6 components
Evaluated models using Bayesian Information Criterion (BIC)
Plotted BIC scores across cluster counts
Key Result:
Lowest BIC observed at 2 clusters
Suggests optimal statistical clustering differs from biological labels
Insight: BIC balances model fit and complexity, often favoring simpler models.
Exercise 4: Effect of Covariance Type
GMMs were fitted using four covariance types:
Covariance Type
Description
full
Each cluster has its own general covariance matrix
tied
All clusters share the same covariance matrix
diag
Diagonal covariance matrices
spherical
Single variance per cluster
Observation:
full covariance provides the most flexible and realistic clusters
spherical produces overly simplistic boundaries
Covariance choice strongly influences clustering behavior
📈 Visual Outputs
PCA scatter plot with true species labels
GMM clustering results on PCA-reduced data
BIC vs number of components line plot
Cluster visualizations for each covariance type
▶️ How to Run the Project
Clone the repository:
Copy code
Bash
git clone https://github.com/your-username/gmm-iris-clustering.git
Install dependencies:
Copy code
Bash
pip install scikit-learn pandas matplotlib numpy
Run the Python script or Jupyter Notebook containing the exercises.
🧠 Key Takeaways
GMMs provide probabilistic clustering, unlike K-Means
PCA helps simplify high-dimensional data for visualization
BIC is a powerful tool for model selection
Covariance type significantly affects clustering geometry
👩🏽‍💻 Author
Lamla Mhlana
Data Science & Machine Learning Learner
ExploreAI Academy
