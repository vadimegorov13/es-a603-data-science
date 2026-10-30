# ES A603 — Fundamentals of Data Science and Engineering

My coursework for ES A603 (Fall 2026): class notebooks, homework, and presentations.

## Homework

| | Project | Dataset |
|---|---|---|
| **HW1** | [Titanic EDA](notebooks/homework/hw1_titanic_eda.ipynb) | [Titanic](https://github.com/mwaskom/seaborn-data) |
| **HW3** | [What makes a Steam game successful?](notebooks/homework/hw3_steam_games_eda.ipynb) | [Steam Games v2](https://www.kaggle.com/datasets/muhammadaqeelkabir/steam-games-dataset-v2) |
| **HW4** | [Regression challenge: predicting superconductor temperature](notebooks/homework/hw4_regression_challenge.ipynb) | [Superconductivity](https://archive.ics.uci.edu/dataset/464/superconductivty+data) |
| **HW5** | [XGBoost vs. the baselines on gas sensor data](notebooks/homework/hw5_xgboost_classification.ipynb) | [Gas Sensor Array Drift](https://archive.ics.uci.edu/dataset/270/gas+sensor+array+drift+dataset+at+different+concentrations) |

Slides for each homework are in [`presentations/`](presentations/).

## Setup

**Recommended (conda):**

```bash
conda env create -f environment.yml
conda activate es603
jupyter lab
```

**Or with pip** (Python 3.11):

```bash
python3.11 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter lab
```

> On a Mac, pip's XGBoost also needs OpenMP: `brew install libomp`. Conda handles this for you.

Homework datasets download automatically when you run the notebooks, so you need an internet connection.
