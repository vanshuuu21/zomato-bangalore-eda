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

1. **Rating Distribution** — Most restaurants cluster around a rating of 3.5–4.2/5, showing most are "decent but not exceptional."
2. **Top Cuisines** — North Indian dominates (2,900+ restaurants), followed by North Indian + Chinese combos and South Indian.
3. **Cost vs Rating** — There is a weak relationship between price and rating — higher prices don't guarantee better ratings.
4. **Online Ordering** — ~58% of restaurants offer online ordering; ratings are similar for those that do vs don't.
5. **Location** — Smaller, less saturated areas have higher average ratings, while BTM and Koramangala have the most restaurants overall.
6. **Restaurant Types** — Quick Bites is the most common format, reflecting Bangalore's fast, casual dining culture.

## 💡 So What?
Cuisine variety and location choice matter more than price or online ordering when it comes to ratings — a useful insight for anyone opening a new restaurant in Bangalore.

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


## 🙋 About Me
Beginner Data Analyst with experience in Power BI and Excel projects, now 
expanding into Python for data analysis and visualization. This project 
marks my first step into Python-based EDA — feedback and suggestions are 
always welcome!
