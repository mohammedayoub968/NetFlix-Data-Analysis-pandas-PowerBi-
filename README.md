# 📊 Netflix Data Analysis with Pandas & Power BI

Welcome to my Netflix Data Analysis project!  
This project is built around a publicly available dataset containing all TV shows and movies available on Netflix as of 2021.

## 📁 About the Dataset
Netflix is one of the world’s largest streaming platforms with over 200 million subscribers. The dataset includes detailed metadata for over 8000 titles including:
- Title
- Type (Movie/TV Show)
- Director
- Cast
- Country
- Date Added
- Release Year
- Rating
- Duration
- Genre (listed_in)
- Description

📌 Dataset Source: [Kaggle Netflix Titles Dataset](https://www.kaggle.com/datasets/shivamb/netflix-shows)

---

## 🧠 Project Objectives
- Understand the structure and features of the dataset.
- Clean and preprocess the data (handle missing values, convert data types, etc.).
- Extract meaningful features for analysis.
- Answer business-driven and exploratory questions:
  - What are the most common genres?
  - Who are the most frequent directors?
  - How has Netflix content grown over the years?
  - What's the typical duration of content?
  - Which countries contribute most to Netflix’s library?

---

## 🔧 Tools & Libraries
- `Python 3.11`
- `Pandas`, `NumPy`
- `Matplotlib`, `Seaborn`
- `Power BI` for dashboarding
- GitHub for version control

---

## 📈 Steps Followed

### 1. Data Loading and Exploration
- Used `.head()`, `.info()`, `.describe()` to inspect the structure.
- Checked for duplicates and missing values.

### 2. Data Cleaning
- Removed leading/trailing whitespaces using `.str.strip()`.
- Converted list-like features (e.g., `cast`, `director`) into actual Python lists.
- Transformed `date_added` to `datetime`.
- Separated `duration` into `duration_value` (numeric) and `duration_unit`.

### 3. Handling Missing Values
- Retrieved missing `director` values via external API (manual effort).
- Remaining missing directors were labeled as `"Unknown"`.
- Filled missing categorical values with mode (e.g., `rating`).

### 4. Feature Engineering
- Exploded lists (e.g., `cast`, `listed_in`) using `.explode()` for granular analysis.
- Calculated metrics such as:
  - Content distribution by type/year
  - Most frequent directors and actors
  - Most common genres
  - Production by country

---

## 📊 Power BI Dashboard
I built an interactive dashboard in Power BI showing:
- Total content breakdown
- Year-over-year growth
- Country-wise production
- Genre distributions
- Duration stats

📸 *Screenshots included in the repo*

---

## 🤝 Acknowledgements
Special thanks to:
- Eng. Ahmed Hafez  
- Eng. Ahmed Hamdy  
for mentoring and guiding throughout the analysis.

Thanks also to **Instant** for allowing me to be part of this wonderful data community.

---

## 📎 Repo Contents
