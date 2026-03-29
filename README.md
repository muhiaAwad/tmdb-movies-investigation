# 🎬 TMDb Movies Dataset Investigation

An exploratory data analysis project investigating factors associated with movie success using The Movie Database (TMDb) dataset.

## 📌 Project Overview

This project explores a dataset of 10,866 movies to uncover what makes a movie financially and critically successful — analyzing the relationship between budget, genre, ratings, and release year.

## ❓ Research Questions

1. **Does a higher production budget lead to a higher movie rating?**
   Exploring the relationship between `budget` and `vote_average`.

2. **What genres generate the highest average profit?**
   Identifying top-performing genres using inflation-adjusted revenue and budget.

3. **Which release year achieved the highest average profit?**
   Exploring how movie profitability has changed over time.

## 📂 Dataset

| Detail | Value |
|--------|-------|
| Source | [TMDb Movies Dataset](https://www.kaggle.com/) |
| Size | 10,866 movies × 21 columns |
| Key columns | `budget`, `revenue`, `vote_average`, `popularity`, `genres`, `release_year`, `director` |

## 🔧 Data Wrangling Steps

- **Missing Values** — Identified and handled null entries
- **Zero Values** — Removed rows with zero budget/revenue (unusable for financial analysis)
- **Data Types** — Fixed incorrect types (dates, numerics)
- **Feature Engineering** — Created `profit` column: `revenue_adj - budget_adj`

## 📊 Key Findings

- 💰 Higher budgets do **not** strongly guarantee higher ratings
- 🎭 Certain genres consistently outperform others in average profit
- 📅 Movie profitability shows clear trends across release years

## 🛠️ Technologies Used

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white)

- **Python** — Data analysis
- **Pandas** — Data cleaning, wrangling, and aggregation
- **Matplotlib / NumPy** — Visualization and statistical summaries
- **Jupyter Notebook** — Analysis environment

## 📁 Project Structure

```
tmdb-movies-investigation/
│
├── Investigate_a_Dataset.ipynb   # Main analysis notebook
├── Investigate_a_Dataset.html    # HTML export for easy viewing
└── README.md
```

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/muhiaAwad/tmdb-movies-investigation.git
   cd tmdb-movies-investigation
   ```

2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib jupyter
   ```

3. Open the notebook:
   ```bash
   jupyter notebook Investigate_a_Dataset.ipynb
   ```

## 📝 Part of

**Udacity Data Analyst Nanodegree** — Investigate a Dataset Project
