# Mexico City Real Estate Analysis

Personal project working through a full data science pipeline on Mexico City real estate listings. Built from scratch with public data.

---

## Where I'm At

- **Part 1: Data Cleaning & Preprocessing** — done ✅
- **Part 2: Visualization & Outlier Treatment** — done ✅
- **Part 3: Correlation & Variable Analysis** — done ✅
- - Part 4: Predictive Modeling — not started yet

---

## The Data

Five CSV files from Properati covering the Mexico City metro area. Combined they had [X] raw listings across 16 features.

---

## Part 1: Cleaning & Preprocessing ✅

Loaded all five files, checked schemas matched, merged into one dataset. Dropped redundant columns, handled nulls, and engineered `lat`, `lon`, and `state` from the location fields.

Ended up with a clean, structured dataset ready for exploration.

---

## Part 2: Visualization & Outlier Treatment ✅

**What I looked at:**
- Histogram of prices
- Histogram of total surface area
- Box plots of price distribution by property type
- Box plots of price distribution by state

**What I found:**
- Heavy right skew in both price and area — a few extreme listings pulling the tail way out

**What I did:**
- Trimmed bottom and top 5% quantiles to remove outliers
- Plotted area vs price scatterplot to see the relationship
- Ran an `sns.regplot` to check the trend line
- Broke out scatterplots for the top 3 states by mean price to compare regional patterns

---

## Tools Used

Python, pandas, matplotlib, seaborn, Jupyter Notebook

---

## What's Next
## Part 3: Correlation & Variable Analysis ✅

- Built full correlation matrix for numeric features
- Computed area-price correlation grouped by state and property type
- Engineered `price_per_m2` feature
- Explored relationship between property size and price efficiency
- Filtered extreme outliers for cleaner visualization
- Part 4: Build a model to predict prices

