🔢 Principal Component Analysis (PCA) on the Digits Dataset

Dimensionality Reduction & Variance Analysis
© ExploreAI Academy

This project applies Principal Component Analysis (PCA) to the Digits dataset to reduce dimensionality, analyse variance distribution, and determine the optimal number of components required to retain meaningful information while improving computational efficiency.




🚀 Project Objectives

This project demonstrates the ability to:

Apply PCA to high-dimensional data

Analyse explained variance and cumulative variance

Determine the minimum number of components needed to retain ≥85% variance

Understand the impact of dimensionality reduction on downstream modeling

Work with image-based datasets in machine learning





📂 Dataset Overview

Digits Dataset

Source: sklearn.datasets.load_digits

1,797 samples

Each image is 8×8 pixels

64 numerical features per sample

Target labels: digits 0–9


Each observation represents a handwritten digit flattened into a 64-dimensional vector.




🛠️ Tools & Libraries

Python 3

NumPy

Pandas

Scikit-learn

Matplotlib





📘 Project Workflow



1️⃣ Data Preparation

Loaded the Digits dataset

Standardized features using StandardScaler

Ensured equal contribution of all pixel values before PCA


📌 Why standardization matters:
PCA is sensitive to feature scale—standardization prevents dominant features from skewing results.



2️⃣ Applying PCA

Applied PCA without specifying components

Allowed PCA to compute all 64 principal components

Transformed standardized data into PCA space





3️⃣ Explained Variance Analysis

Calculated explained variance ratio for each component

Observed:

PC1 explains ~12% of variance

Variance is distributed across many components

No single component dominates



📌 Insight:
Handwritten digit images contain complex patterns spread across multiple dimensions.



4️⃣ Cumulative Variance Evaluation

Computed cumulative explained variance

Determined how variance accumulates as components increase


📈 Key Result:
➡️ 25 principal components capture ~85% of total variance



5️⃣ Optimal Component Selection

Variance Threshold	Components Required

50%	~8 components
75%	~18 components
85%	25 components
95%	~40 components


📌 Conclusion:
Retaining 25 components provides a strong balance between information retention and dimensionality reduction.



🧠 Impact on Modeling & Analysis

✅ Benefits

Dimensionality Reduction: 64 → 25 features

Lower Risk of Overfitting: Reduced noise and redundancy

Improved Computational Efficiency

Better Generalization

Easier Visualization (for low-component projections)


⚠️ Considerations

PCA components are not directly interpretable

Must validate performance on downstream models

Task-dependent trade-off between accuracy and compression





📈 Practical Applications

Image classification

Feature extraction

Noise reduction

Preprocessing for clustering or neural networks

Exploratory data analysis on high-dimensional datasets





💼 Portfolio Value

This project demonstrates:

✔ Strong understanding of linear algebra concepts in ML
✔ Data preprocessing best practices
✔ Model-agnostic feature engineering
✔ Analytical decision-making using variance metrics

Ideal for:

Data Science roles

Machine Learning internships

Computer Vision foundations

Applied AI portfolios




👩🏽‍💻 Author

Lamla Mhlana
Aspiring Data Scientist | Machine Learning Enthusiast
ExploreAI Academy| Alx Academy 


