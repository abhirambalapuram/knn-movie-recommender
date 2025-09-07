# KNN Movie Recommender

A simple movie recommendation system built using the MovieLens dataset. This project combines exploratory data analysis (EDA) with a K-Nearest Neighbors (KNN) model to recommend movies based on similarity of user ratings.


**Project Overview**

Recommender systems are a cornerstone of modern data science, widely used in streaming platforms like Netflix, Amazon Prime, and YouTube. In this project, we:

Performed EDA to understand user behavior and movie rating distributions.

Analyzed genre-level patterns, identifying which genres tend to receive higher ratings.

Built an item-based KNN recommender that finds movies similar to a given input using cosine similarity on the user–item rating matrix.

Provided an easy-to-use function that outputs the top-N most similar movies to any queried title.


**Exploratory Data Analysis (EDA)**

Key insights from the dataset:

Rating Distribution: Most users tend to rate movies between 3 and 4 stars.

Top Rated Movies: Popular classics such as Toy Story (1995), Star Wars (1977), and The Matrix (1999) dominate in number of ratings.

Genre Trends: Certain genres (e.g., Documentaries and Dramas) show higher average ratings, while others (e.g., Horror, Action) vary widely.

Visualizations include:

Histogram of rating distribution

Bar chart of top 10 most rated movies

Average rating by genre


**Machine Learning Model**

We applied Item-Based Collaborative Filtering using K-Nearest Neighbors (KNN):

Input: User–movie rating matrix (sparse matrix form).

Similarity Metric: Cosine similarity between movie rating vectors.

Model: sklearn.neighbors.NearestNeighbors.

Output: A ranked list of movies most similar to the given title.



**Example Output**

Input Movie: Toy Story (1995)

Top 5 Recommendations:
1. Aladdin (1992) — similarity: 0.93
2. Lion King, The (1994) — similarity: 0.91
3. Beauty and the Beast (1991) — similarity: 0.90
4. Hercules (1997) — similarity: 0.88
5. Aladdin and the King of Thieves (1996) — similarity: 0.87


**Dataset**

MovieLens Latest Small Dataset (ml-latest-small)

~100,000 ratings from ~600 users on ~9,000 movies

Includes movie metadata (titles, genres)

https://grouplens.org/datasets/movielens/


**Tech Stack**

Python: Data processing and modeling

Pandas & NumPy: Data wrangling

Matplotlib & Seaborn: Visualization

Scikit-learn: KNN algorithm and similarity measures
