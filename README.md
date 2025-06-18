# Netflix-Data-Cleaning-Analysis-and-Visualization

## 📌 Project Overview

This project focuses on cleaning, analyzing, and visualizing data from Netflix's content catalog using Python libraries such as Pandas, Matplotlib, and Seaborn. The dataset includes Netflix titles released or added between 1925 and 2021. The goal is to explore the dataset, derive meaningful insights, and establish a foundation for potential machine learning applications.

---

## 🔧 Tools & Technologies

- **Python** (Pandas, NumPy, Matplotlib, Seaborn)
- **Jupyter Notebook / Google Colab**
- **CSV Dataset**: Netflix titles from Kaggle (cleaned version)

---

## 🧹 Data Cleaning

- Checked for null values across all columns.
- Standardized and handled placeholder entries such as `"Not Given"`.
  - **Director** column: 29.44% missing; imputed as `"Unknown"` to preserve rows.
  - **Country** column: 3.27% missing; rows dropped due to low impact.
- Removed duplicate rows (none found).
- Converted `date_added` column from object to datetime format.

---

## 📊 Exploratory Data Analysis (EDA)

### 1. Content Type Distribution
- Movies significantly outnumber TV Shows on the platform, indicating a preference for short-form content.

### 2. Country-wise Content Production
- The United States leads in content contribution, followed by India and the United Kingdom, reflecting Netflix’s core markets and strategic content partnerships.

### 3. Genre Distribution
- Common genres include Drama, Comedy, and International Movies.
- Titles often span multiple genres, enhancing searchability and viewer targeting.

### 4. Content Addition Over Time
- Steady increase in content, peaking during 2019–2020, suggesting aggressive content expansion and original productions.

### 5. Ratings Analysis
- Most content is targeted toward mature audiences with high occurrences of TV-MA and TV-14 ratings.

### 6. Movie Duration Distribution
- Majority of movies fall within the 80–120 minute range, aligning with standard feature-length films.

### 7. Top Directors (Excluding "Unknown")
- After filtering out unknown entries, directors such as Rajiv Chilaka and Alastair Fothergill were most featured, highlighting popularity of children’s content and documentaries.

---

## 📌 Key Insights

- Netflix focuses more on movies than TV series.
- The platform’s content is heavily skewed toward adult audiences.
- There is a strong representation of U.S.-based content.
- Genre tagging is broad, aiding discoverability.
- Several directors have contributed a high volume of titles, often within niche genres.

---

## 📁 Project Structure
netflix_project/
│
├── netflix_data.csv
├── cleaned_netflix_data.csv
├── netflix_eda.ipynb
├── README.md

---

## 📈 Future Enhancements

- Develop content-based or collaborative filtering recommender systems.
- Perform clustering on genres or countries for market segmentation.
- Apply predictive models for content success or genre forecasting.

---

## 📚 References

- Dataset: [Kaggle - Netflix Titles Dataset](https://www.kaggle.com/datasets/shivamb/netflix-shows)
- Visualizations inspired by public Tableau dashboards and EDA guides

---

## Author

This project was developed as part of a learning portfolio in data analysis and visualization using real-world entertainment datasets.


