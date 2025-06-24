# 🎬 Genre Success Analysis in 21st Century Cinema

This project explores the success of various film genres in the 21st century using data from IMDb. It evaluates genres based on **audience rating**, **box office performance**, and **award achievements**, and visualizes the findings through an interactive Tableau dashboard.

## 📈 Problem Overview

In a rapidly evolving film industry, determining which genres are most successful is not straightforward. While some genres dominate box office sales, others shine through critical acclaim or audience appreciation. This project aims to identify those patterns by analyzing multiple dimensions of success.

## 🧹 Data Cleaning & Transformation (in Python)

1. Loaded raw Excel data using `pandas`, previewed with `.head()`.
2. Checked for and confirmed **no duplicate entries**.
3. Identified columns with over **50% missing values** and removed them (e.g., Language 2–15, Director 2–3, etc.).
4. Imputed missing values in remaining columns:
   - **Numerical columns**: filled with **median** (due to skewed distribution).
   - **Categorical columns**: filled with **mode**.
5. Saved the cleaned dataset as `IMDB_data_clean.csv`.

## 📊 Dashboard Creation in Tableau

After cleaning, the data was used to build an interactive dashboard in Tableau Public:
- Created calculated fields (e.g., `MOVIE_REVENUE_CATEGORY`, `IS_AWARD_WINNER`, `YEARS_SINCE_RELEASE`) for deeper insights.
- Built multiple visualizations:
  - IMDb Rating per Genre
  - Total Box Office per Genre
  - Total Awards per Genre
  - Correlation between MetaScore and Box Office
- Combined visuals into a single dashboard to tell a complete story.

## 📚 Insights Summary

- **Action** films lead commercially, generating the highest total revenue.
- **Drama** dominates in award wins, showing critical recognition.
- **Mystery** films earn the highest average IMDb rating, favored by audiences.
- High box office performance does **not** always correlate with high critical ratings (MetaScore).

## 📌 Tools Used

- **Python** (pandas) – for data cleaning
- **Tableau Public** – for visualization
