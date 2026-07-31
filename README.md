# 🍽️ Zomato Bangalore — Exploratory Data Analysis

A beginner data analytics project exploring restaurant trends in Bangalore using the Zomato dataset — cleaning raw data, uncovering patterns in ratings, cuisines, cost, and online ordering, and visualizing the findings.

## 📌 Project Overview
This project analyzes ~51,000 restaurant listings from Zomato to answer:
- What does the overall rating distribution look like?
- Which cuisines and restaurant types are most common?
- Does cost correlate with rating?
- Does offering online ordering relate to better ratings?
- Which locations have the highest-rated restaurants?

## 🛠️ Tech Stack
- Python
- pandas, numpy — data cleaning & manipulation
- matplotlib, seaborn — visualization
- Jupyter Notebook / Google Colab

## 📂 Repo Structure
```
zomato-eda/
├── README.md
├── requirements.txt
├── notebook/
│   └── zomato_eda.ipynb
├── data/
│   └── zomato.csv          # not included — see Data section below
└── images/
    └── (exported chart screenshots, optional)
```

## 📊 Key Insights
> Fill this in after running the notebook — see the storytelling notes below.

1. **Rating Distribution** — most restaurants rate between ___–___/5.
2. **Top Cuisines** — ___ dominates, followed by ___.
3. **Cost vs Rating** — [weak / no / moderate] relationship between price and rating.
4. **Online Ordering** — ___% of restaurants offer it; ratings are [higher/similar/lower] for those that do.
5. **Location** — ___ has the highest average rating among top areas.
6. **Restaurant Types** — ___ is the most common format.

## 🧹 Data Cleaning Steps
- Removed duplicate rows
- Dropped irrelevant columns (`url`, `address`, `phone`, `menu_item`, `reviews_list`)
- Cleaned `rate` column (removed `/5`, handled `NEW`/`-`/missing values)
- Cleaned `approx_cost(for two people)` (removed commas, converted to numeric)
- Standardized `cuisines` text (lowercase, trimmed)

## 📈 Visualizations
- Distribution of ratings (histogram + KDE)
- Top 10 cuisines (bar chart)
- Cost vs rating (scatterplot)
- Online order availability (countplot)
- Top 10 restaurant types (bar chart)
- Correlation heatmap (rating, votes, cost)
- Average rating by location (bar chart)
- Rating by online order availability (boxplot)

## 📁 Data
The dataset (`zomato.csv`) is not included due to size/licensing. Download it from [Kaggle — Zomato Bangalore Restaurants](https://www.kaggle.com/datasets/himanshupoddar/zomato-bangalore-restaurants) and place it in the `data/` folder.

## ▶️ How to Run
```bash
git clone https://github.com/<your-username>/zomato-eda.git
cd zomato-eda
pip install -r requirements.txt
jupyter notebook notebook/zomato_eda.ipynb
```

## 🙋 About Me
Beginner Data Analyst python, EDA, and data visualization. Feedback welcome!
