
# 🎬 In-Depth Analysis of Box Office Films

## About This Project

Hi, I'm **Stephen**, and this project represents my end-to-end analysis of the movie industry. By examining box office performance, genre trends, audience ratings, and production budgets, I aimed to answer a key business question:

> **If a new movie studio wants to enter the industry, what types of films should they create for maximum success?**

This project combines data exploration, statistical testing, and predictive modeling to reveal meaningful insights and actionable recommendations.

---

## 🎯 The Challenge

A new studio with no prior industry experience needs guidance on what kinds of films to produce. My goal was to break down the industry using real data and uncover the factors behind high-performing movies.

### My Core Objectives

1. Identify **top-performing film genres**
2. Analyze **current box office trends**
3. Determine the **key drivers** behind movie success
4. Convert insights into **clear, practical business strategies**

---

## 📊 Data Sources

To ensure a robust understanding of the industry, I used multiple high-quality datasets:

* **bom.movie_gross.csv** — Domestic & international box office data
* **tmdb.movies.csv** — Popularity metrics, user ratings, and movie details from TMDB
* **tn.movie_budgets.csv** — Production budgets and gross revenue
* **im.db (SQLite)** — IMDb movie basics, genres, runtimes, ratings, and vote counts

These diverse datasets allowed a holistic analysis from financial, genre-based, and audience perspectives.

---

## 🔧 My Approach

### 1. Data Preparation & Cleaning

I invested significant effort into preparing clean, analysis-ready data:

* Removed duplicates and filled missing values
* Cleaned financial columns (removed `$`, `,`, cast to numeric)
* Converted dates and extracted release years/months
* Engineered key KPIs: **profit**, **profit ratio**, **total gross**
* Merged multiple datasets into unified DataFrames like `df_box` and `combined_data_with_budget`

---

### 2. Exploratory Data Analysis (EDA)

My analysis included:

* **Financial Performance:** Profitability, high-grossing films, studio comparisons
* **Genre Analysis:** Distribution patterns, rating trends, performance patterns
* **Temporal Trends:** Release timing, yearly patterns, seasonal performance
* **Budget Dynamics:** Impact of budget on revenue and ROI
* **Market Behavior:** Domestic vs. foreign market contributions

---

### 3. Statistical Hypothesis Testing

To validate assumptions:

1. **Domestic vs. Foreign Gross – Paired t-test**
   → Significant difference: foreign markets are crucial

2. **Studio Profitability – ANOVA**
   → No significant differences: studio brand ≠ profitability

3. **Budget vs. ROI – Independent t-test**
   → High-budget films have *lower* ROI than low-budget ones

4. **Genre vs. Ratings – ANOVA**
   → Significant differences: Documentaries & Dramas rate highest

---

### 4. Predictive Modeling

A Linear Regression model was built to predict **worldwide gross** using **production budget**.

* **R² Score:** 0.58
* **RMSE:** $138.61M
* **Key Insight:**
  Each **$1M increase in production budget → ~$3.31M increase in worldwide gross**
  (Budget strongly influences performance, but it’s not the only factor.)

---

## 💡 Key Discoveries

1. **Top Genres Perform Differently**

   * Highest grossing: **Action, Adventure, Animation**
   * Highest rating: **Documentary, Drama**

2. **The Budget Paradox**

   * High-budget films = high revenue
   * But low-budget films = *higher ROI*

3. **International Markets Dominate**

   * Foreign gross often exceeds domestic
   * Global appeal is essential for blockbusters

4. **Studio Brand Does Not Guarantee Success**

   * Profitability varies more by **project selection**

5. **Release Timing Matters**

   * Best months: **May, June, July, November, December**

---

## 🎬 My Recommendations

* **Smart Budgeting:** Focus on **mid-budget films** ($30M–$80M)
* **Genre Strategy:**

  * Commercial hits: **Action, Adventure, Animation**
  * Critical success: **Documentary, Drama**
* **Think Global:** Build stories that resonate internationally
* **Strategic Timing:** Release in **Summer or Holiday** windows

---

## 🛠️ Technologies & Tools

* **Python 3.x**
* Pandas, NumPy
* Matplotlib, Seaborn
* SciPy, StatsModels
* scikit-learn
* SQLite
* Jupyter Notebook

---

## 📁 Project Structure

```
├── Data/                              
├── movie_industry_analysis.ipynb     # Main (and only) notebook
├── README.md                          
└── Cleaned_Data/                      
```

---

## 📈 Interactive Dashboard

Explore the visuals here:

👉 **[https://public.tableau.com/app/profile/stephen.muema/viz/MovieIndustryAnalysis_17630239953860/MovieIndustryAnalysis?publish=yes](https://public.tableau.com/app/profile/stephen.muema/viz/MovieIndustryAnalysis_17630239953860/MovieIndustryAnalysis?publish=yes)**

---

## 🚀 Getting Started

1. Clone the repository
2. Install Python 3.x and requirements
3. Open `movie_industry_analysis.ipynb`
4. Run cells sequentially to reproduce the analysis

---

## 📫 Connect With Me

I’m passionate about transforming data into meaningful business insights. If you’d like to collaborate or discuss this project, feel free to reach out.

---

**Built with curiosity, data, and ☕ by Stephen Musyoka.**
*This project showcases my full data analysis workflow — from cleaning and exploration to statistical testing, modeling, and strategic recommendations.*

---

