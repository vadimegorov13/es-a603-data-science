# ES A603 — Fundamentals of Data Science and Engineering

Coursework for ES A603 (Fall 2026): in-class notebooks, homework assignments, and homework presentations.

## Repository structure

```
.
├── data/                  # CSV datasets used by the class notebooks
├── notebooks/
│   ├── class/             # My in-class notebooks (weeks 1–5, days 14 & 16)
│   ├── homework/          # Homework assignments
│   └── instructor/        # Instructor-provided notebooks (days 6–9, written for Google Colab)
├── presentations/         # Homework slide decks (.pptx, plus Keynote originals)
└── requirements.txt
```

## Homework

| # | Notebook | Topic | Dataset |
|---|----------|-------|---------|
| 1 | [hw1_titanic_eda](notebooks/homework/hw1_titanic_eda.ipynb) | Exploratory data analysis with pandas & matplotlib | [Titanic (seaborn-data)](https://github.com/mwaskom/seaborn-data) |
| 3 | [hw3_steam_games_eda](notebooks/homework/hw3_steam_games_eda.ipynb) | EDA: what characteristics relate to a game's success on Steam? | [Steam Games Dataset v2 (Kaggle)](https://www.kaggle.com/datasets/muhammadaqeelkabir/steam-games-dataset-v2) |
| 4 | [hw4_regression_challenge](notebooks/homework/hw4_regression_challenge.ipynb) | Linear, Polynomial, Ridge and Lasso regression compared | [Superconductivity Data (UCI)](https://archive.ics.uci.edu/dataset/464/superconductivty+data) |
| 5 | [hw5_xgboost_classification](notebooks/homework/hw5_xgboost_classification.ipynb) | XGBoost vs. Logistic Regression and Decision Tree | [Gas Sensor Array Drift (UCI)](https://archive.ics.uci.edu/dataset/270/gas+sensor+array+drift+dataset+at+different+concentrations) |

Slides for each assignment are in [`presentations/`](presentations/).

## Datasets in `data/`

- `Student_Performance.csv` — student performance regression data
- `lung_cancer_dataset.csv` — lung cancer classification data
- `healthcare-dataset-stroke-data.csv` — stroke prediction data

Homework datasets are downloaded at runtime (via URL, `kagglehub`, or `ucimlrepo`), so they are not stored here.

## Setup

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter lab
```

Notebooks read data with paths relative to their own folder (`../../data/...`), so launch them from inside `notebooks/<subfolder>/` (Jupyter and VS Code do this by default).

The instructor notebooks were written for Google Colab and use `google.colab.files.upload()`; when running locally, skip that cell — the data paths already point to `data/`.

## Author

Vadim Egorov
