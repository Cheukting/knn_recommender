# KNN Recommender

By using [MovieLens Datasets](https://grouplens.org/datasets/movielens/latest/) we build a recommender system based on KNN Item-Based Collaborative Filtering.

## Enviroment Setup

Use [poetry](https://python-poetry.org/) to set up the Python environment (Python >= 3.9)

Get the full data set from [MovieLens Datasets](https://grouplens.org/datasets/movielens/latest/) and put the `movies.csv` and `ratings.csv` in this repo.

## Complete the exercises

Find all the `TODO` comments in `knn_recommender.py` and finish the missing pieces in the code. The finished version is in the [finished branch](https://github.com/Cheukting/knn_recommender/tree/finished)

## Run in CLI

Run the `knn_recommender.py` with the following optional options:

* `--movie_name` : provide your favoriate movie name
* `--top_n` : top n movie recommendations
* `--path` : input data path, default to be `./`
* `--movies_filename` : default to be `movies.csv`
* `--ratings_filename` : default to be `ratings.csv`

Example:

`python knn_recommender.py --movie_name "Iron Man" --top_n 10`

## Run in Browser

*Make sure you have run it once in the CLI and have the pickle files (`hashmap.p` and `movie_user_mat_sparse.p`) in this repo*

Start a local webserver:

`python -m http.server`

Open [http://0.0.0.0:8000](http://0.0.0.0:8000) and select `knn_recommender.html` from there

---

*Credit to Kevin Laio ([KevinLiao159](https://github.com/KevinLiao159)) for [original code](https://github.com/KevinLiao159/MyDataSciencePortfolio/blob/master/movie_recommender/src/knn_recommender.py) and [blog post](https://towardsdatascience.com/prototyping-a-recommender-system-step-by-step-part-1-knn-item-based-collaborative-filtering-637969614ea)*
