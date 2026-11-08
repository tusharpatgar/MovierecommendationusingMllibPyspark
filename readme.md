# Movie Recommendation System with PySpark MLlib

A notebook-based movie recommendation experiment using Apache Spark MLlib's Alternating Least Squares (ALS) collaborative-filtering algorithm.

## Overview

The project uses movie metadata and user ratings to train an ALS model, predict ratings, and evaluate prediction error with Root Mean Squared Error (RMSE).

## Dataset

The `datasets/` directory contains:

- `movies.csv` — movie identifiers and movie metadata.
- `ratings.csv` — user/movie rating records.

Keep the dataset files in this directory or update the notebook paths to match your environment.

## Technology

- Python
- Apache Spark / PySpark
- Spark MLlib
- ALS collaborative filtering
- Jupyter Notebook

## Getting started

### Requirements

- Python 3
- Java runtime compatible with your installed Spark version
- Jupyter Notebook
- PySpark

Install the Python packages:

```bash
python -m pip install pyspark notebook
```

### Run the notebook

1. Clone this repository.
2. Start Jupyter from the repository root.
3. Open `Recommendation.ipynb`.
4. Verify the dataset paths point to `datasets/movies.csv` and `datasets/ratings.csv`.
5. Run the notebook cells in order.

```bash
jupyter notebook Recommendation.ipynb
```

## Workflow

1. Load movie and rating data into Spark.
2. Prepare the user, movie, and rating columns required by ALS.
3. Split ratings into training and test sets.
4. Train an ALS recommendation model.
5. Generate predictions for held-out ratings.
6. Evaluate prediction error using RMSE.

## Repository structure

```text
datasets/
  movies.csv
  ratings.csv
Recommendation.ipynb
README.md
```

## Limitations

This is a learning project, not a deployed recommendation service. Model quality depends on the dataset, train/test split, ALS parameters, and handling of unseen users or movies. Review the notebook for its exact preprocessing and evaluation choices.

## License

No license is currently specified. Contact the repository owner before reusing the contents.
