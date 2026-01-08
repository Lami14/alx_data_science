Advanced Dimensionality Reduction Techniques
Exercise: Advanced Dimensionality Reduction Techniques
© ExploreAI Academy
This project explores advanced dimensionality reduction methods—PCA, MDS, and t-SNE—and applies them to the Wine dataset to visualize high-dimensional data in two dimensions.
🎯 Learning Objectives
By completing this exercise, you will be able to:
Understand the theory behind PCA, MDS, and t-SNE
Apply dimensionality reduction techniques to real datasets
Visualize high-dimensional data in 2D space
Interpret variance, stress values, and clustering behavior
📂 Dataset
The Wine dataset from sklearn.datasets is used in all exercises.
Dataset characteristics:
178 samples
13 numerical features
3 wine classes
🛠️ Technologies Used
Python 🐍
Scikit-learn
Matplotlib
NumPy
📊 Exercises Overview
Exercise 1: Principal Component Analysis (PCA)
Reduced the dataset to 2 principal components
Explained variance ratio:
PC1 ≈ 99.81%
PC2 ≈ 0.17%
Visualization shows reasonable class separation, indicating PCA effectively captures most variance in the first component.
Key Insight:
PCA preserves global variance structure but may not always separate classes optimally.
Exercise 2: Multi-Dimensional Scaling (MDS)
Reduced data to 2 dimensions
Stress value obtained:
Copy code

19573.00
MDS preserves pairwise distances, revealing clusters but with some overlap.
Key Insight:
Lower stress values indicate better distance preservation. MDS is useful for similarity-based visualizations.
Exercise 3: t-Distributed Stochastic Neighbour Embedding (t-SNE)
Reduced data to 2 dimensions
Computation time:
Copy code

~1.69 seconds
Resulting plot shows clear and well-separated clusters
Key Insight:
t-SNE excels at revealing local structures and clusters but is computationally more expensive and non-deterministic.
📈 Visual Outputs
PCA scatter plot
MDS scatter plot
t-SNE scatter plot
Each plot colored by wine class
▶️ How to Run the Code
Clone the repository:
Copy code
Bash
git clone https://github.com/your-username/advanced-dimensionality-reduction.git
Install dependencies:
Copy code
Bash
pip install scikit-learn matplotlib
Run the Python script or Jupyter Notebook containing the exercises.
🧠 Key Takeaways
Technique
Strength
Limitation
PCA
Fast, explains variance
Linear, less effective for complex clusters
MDS
Preserves distances
Computationally expensive
t-SNE
Excellent clustering
Slow, not suitable for large datasets
