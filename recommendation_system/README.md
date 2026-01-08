🎬 Content-Based Recommender System (Netflix Titles)

Unsupervised Learning & NLP Project
© ExploreAI Academy

This project implements a content-based recommendation system using a dataset of Netflix movies and TV shows. By leveraging text preprocessing, TF-IDF vectorization, and cosine similarity, the system recommends titles similar to a given show based on content attributes such as genre, cast, title, and description.


---

🚀 Project Objectives

This project demonstrates the ability to:

Understand and implement content-based recommendation systems

Clean and preprocess real-world text data

Convert text data into numerical representations using TF-IDF

Measure similarity using cosine similarity

Build and test a recommendation function

Generate meaningful recommendations without user interaction data



---

📂 Dataset Overview

Netflix Titles Dataset

Source: ExploreAI Public Data Repository

Each record represents a movie or TV show available on Netflix.

Key attributes used:

title

type (Movie or TV Show)

cast

listed_in (genres/categories)

description


The dataset provides rich textual metadata, making it well-suited for content-based filtering.


---

🛠️ Tools & Libraries

Python 3

NumPy

Pandas

Scikit-learn

Regular Expressions (re)



---

📘 Project Workflow


---

1️⃣ Data Cleaning & Preprocessing

To ensure high-quality recommendations, the following steps were applied:

Removed rows with missing values in key text columns

Cleaned text by:

Removing punctuation and non-alphanumeric characters

Normalising whitespace


Special handling for the cast column:

Removed spaces within names

Replaced commas with spaces to treat actor names as individual tokens



📌 Why this matters:
Text consistency reduces noise and improves similarity calculations.


---

2️⃣ Feature Engineering

Combined the following columns into a single textual feature:

listed_in

cast

title

description


Dropped irrelevant metadata columns

Final dataset retained:

type

title

combined (main feature for similarity computation)



📌 Result:
Each title is represented by a rich, unified textual profile.


---

3️⃣ Text Vectorization with TF-IDF

Applied TF-IDF Vectorization to the combined text feature

Converted text into numerical vectors representing word importance

Used default unigram settings


📌 Advantage:
TF-IDF reduces the impact of common words while emphasising distinctive terms.


---

4️⃣ Similarity Computation

Computed cosine similarity between all TF-IDF vectors

Produced a similarity matrix capturing pairwise title similarities


📌 Interpretation:
Higher cosine similarity scores indicate stronger content resemblance.


---

5️⃣ Recommendation Function

Implemented a function that:

Accepts a title as input

Identifies its index in the dataset

Retrieves and sorts similarity scores

Returns the top 10 most similar titles


The function also gracefully handles cases where a title is not found.


---

6️⃣ Model Testing

Test Case:
Input title: The Crown

Sample Recommendations:

Reign

London Spy

Planet Earth: The Complete Collection

The Blue Planet

Witches: A Century of Murder


📌 Observation:
The recommendations align well with historical, political, and documentary-style content, indicating effective content matching.


---

🧠 Key Learnings

Content-based systems work well without user ratings

Text preprocessing significantly affects recommendation quality

TF-IDF + cosine similarity is a strong baseline for recommender systems

Combining multiple text attributes improves contextual understanding

Such systems can suffer from limited novelty (recommendations stay close to known preferences)



---

📈 Applications

Streaming platforms (Netflix, Amazon Prime, Showmax)

News and article recommendation

E-learning content suggestions

Book and media discovery platforms



---

💼 Portfolio Value

This project demonstrates:

✔ Natural Language Processing (NLP) fundamentals
✔ Recommendation system design
✔ Feature engineering with text data
✔ Real-world dataset handling
✔ Clean, modular Python implementation

Suitable for:

Data Science roles

Machine Learning internships

AI / Recommendation Systems portfolios



---

👩🏽‍💻 Author

Lamla Mhlana
Aspiring Data Scientist | Machine Learning Enthusiast
ExploreAI Academy | ALX Academy 


