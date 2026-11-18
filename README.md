# Movie Recommender (Item-Based)

Recommends movies that are **similar to a chosen movie**, based on how users rated them.

> 📚 **Course project:** completed while following the Udemy course *Python for Data Science and Machine Learning Bootcamp* (Pierian Data). The dataset and task come from the course.

## Data
- `u.data`: user ratings (user id, movie id, rating, timestamp)
- `Movie_Id_Titles`: movie id → title

## Approach
1. Merged ratings with movie titles and calculated the average rating and number of ratings per movie
2. Built a **user × movie rating matrix** (pandas `pivot_table`)
3. Found similar movies by **correlating rating vectors** (`corrwith`)
4. Filtered out movies with too few ratings, so the recommendations are reliable

## Possible next steps
Collaborative filtering with matrix factorization (e.g. SVD), and evaluation with a held-out test set.

## Tech
Python · pandas · NumPy · Matplotlib · Seaborn · Jupyter

## Run it
```bash
git clone https://github.com/Aniket1103200/movie-recommender-basic.git
cd movie-recommender-basic
pip install -r requirements.txt
jupyter notebook movie_recommender.ipynb
```
