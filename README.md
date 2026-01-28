# 🎬 Investigating Movie Duration Trends & Short Action Movies from the 1990s (Netflix Catalog)

## 📌 Project Overview
Netflix began in 1997 as a DVD rental service and has since grown into one of the world’s largest entertainment platforms. With thousands of titles available, the Netflix catalog provides a strong foundation for applying **exploratory data analysis (EDA)** techniques to uncover trends in the entertainment industry.

In this project, I analyzed **movie duration trends**, with a specific focus on:
- Movies released in the **1990s**
- The prevalence of **short action movies (< 90 minutes)** during that decade  

This analysis was conducted from the perspective of a **production company specializing in nostalgic styles**, seeking insights that could inform modern content strategy.

---

## 🎯 Objectives
- Explore Netflix movie duration trends  
- Analyze movies released before the year 2000  
- Identify short action movies from the 1990s  
- Engineer meaningful genre categories  
- Communicate insights through data visualization  

---

## 📂 Dataset
**File:** `netflix_data.csv`  

The dataset contains **4,812 records** and **11 fully populated columns**.

### Dataset Description
| Column | Description |
|------|-------------|
| show_id | Unique show identifier |
| type | Movie or TV Show |
| title | Title |
| director | Director |
| cast | Cast members |
| country | Country of origin |
| date_added | Date added to Netflix |
| release_year | Year of release |
| duration | Duration in minutes |
| description | Show summary |
| genre | Genre |

---

## 🛠 Tools & Technologies
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**

---

## 🔍 Exploratory Data Analysis

### Data Quality Checks
- Release years ranged from **1942–2021**
- Movie durations ranged from **1–253 minutes**
- No missing values detected across all columns

---

## 🎭 Feature Engineering: Genre Categorization
A new column, **`Main_genre`**, was created by grouping Netflix’s detailed genre labels into broader analytical categories:
- Drama  
- Comedy  
- Action  
- Horror  
- Documentary  
- Children & Family  
- International & Cultural  
- Reality TV  
- Other  

This enabled clearer aggregation and visualization across content types.

---

## 📊 Project Visualizations
All visual outputs are saved in the repository and included below.

### Genre Distribution on Netflix
!<img width="1247" height="595" alt="image" src="https://github.com/user-attachments/assets/8749e1f9-e137-4534-8aee-1d0deaa245a5" />


### Main Genre Breakdown
!<img width="1247" height="571" alt="image" src="https://github.com/user-attachments/assets/3e27a88b-55f8-48dd-b8cd-11c81c8aa163" />


### Movie Duration Distribution (Pre-2000)
!<img width="842" height="545" alt="image" src="https://github.com/user-attachments/assets/46400e59-7e36-4b9e-baf3-a700d1137aca" />


### Short Action Movies in the 1990s
!<img width="846" height="545" alt="image" src="https://github.com/user-attachments/assets/46f0d487-8a95-49e3-ba86-1d7fa3612ae3" />


> 📁 **Visuals Folder:**  
> All charts can be found in the `/visuals` directory.

---

## 📈 Key Findings

### 🎥 Movie Duration Trends
- Average movie duration is approximately **100 minutes**
- Movies released before 2000 show wide variability, including long-form classics

### ⚡ Short Action Movies (1990s)
- **13 action movies** released in the 1990s were under **90 minutes**
- Most short action movies clustered around **88–89 minutes**
- Production spanned multiple regions, including the **US, Hong Kong, and Japan**

These findings indicate that **short, fast-paced action films were a consistent format in 1990s cinema**, particularly within international markets.

---

## 📁 Repository Structure
```text
├── netflix_data.csv
├── netflix_eda.ipynb
├── visuals/
│   ├── genre_distribution.png
│   ├── main_genre_distribution.png
│   ├── 1990s_movie_duration.png
│   └── short_action_movies_1990s.png
└── README.md
