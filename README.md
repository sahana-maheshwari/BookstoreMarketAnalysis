# Massachusetts Bookstore Market Analysis

An exploratory data analysis of independent bookstores across Massachusetts, profiling how store characteristics relate to local income and literacy in order to inform a new book-product market-entry decision.

Team project for the **Business Analytics (client)** course at Hult International Business School.

---

## The problem

A client wanted to understand where a new book product could land. The analysis focused on identifying bookstores that carry an **"early chapter" section** and on profiling the towns around them, so the client could target the right segments and geographies.

## The approach

- **Dataset construction:** an initial attempt using the top/bottom 10 ZIP codes failed because many listed stores were closed or did not exist. The approach was refined to the **top 20 and bottom 20 ZIP codes by income**, producing a clean 40-ZIP dataset.
- **Variables:** ZIP, town, income level, bookstore names, presence of an early-chapter section (Y/N), square footage, presence of a cafe (Y/N), and monthly events hosted.
- **Data hygiene:** ZIP codes cast to 5-digit strings with leading-zero padding so codes like `01103` are not misread as integers.
- **Analysis:**
  - Univariate — histograms and boxplots of numeric columns.
  - Bivariate — correlation heatmap, scatter plots, and linear regression.
  - Multivariate — encoded scatter plots (e.g. square footage by store, colored by cafe presence; store count by ZIP, colored by income and sized by population).

## Deliverables

- [`bookstore_market_analysis.ipynb`](bookstore_market_analysis.ipynb) — the full Python EDA notebook.

## Stack

- Python — pandas, matplotlib, seaborn (univariate, bivariate, and multivariate analysis)
