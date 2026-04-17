# 🎮 Video Game Sales Analysis

> Exploratory Data Analysis (EDA) of historical video game sales data to identify patterns that determine commercial success across platforms, genres, and regions.

---

## 🛠️ Tools & Technologies

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge&logo=python&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=for-the-badge&logo=scipy&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

---

## 📫 Contact

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/bladimir-andres-hernandez-a1764a2b7)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:bladimir4hernandez@gmail.com)

---

## 📌 Project Overview

This project analyzes a dataset containing information about video games released between **1980 and 2016**, including sales data by region, critic and user scores, genres, platforms, and ESRB ratings.

The goal is to uncover what factors drive a video game's commercial success and provide actionable insights for marketing and product decisions in the gaming industry.

---

## 🎯 Key Questions Answered

- Which platforms generate the most global sales?
- Is there a correlation between critic/user scores and sales?
- Which genres perform best in each region (NA, EU, JP)?
- Do ESRB ratings influence purchasing behavior by region?
- Are the average user ratings for Action and Sports games statistically different?
- Are the average ratings of Xbox One and PC users the same?

---

## 🔍 Methodology

```
1. Data Loading & Exploration
2. Data Cleaning
   - Removed rows with missing game names
   - Filled missing release years with the column mean
   - Converted 'tbd' User Score values to NaN
   - Standardized column names to lowercase
3. Feature Engineering
   - Created a new 'total_sales' column (NA + EU + JP + Other)
4. Exploratory Data Analysis
   - Sales trends by year and platform
   - Platform lifespan analysis
   - Regional preferences (platforms, genres, ESRB ratings)
   - Correlation between scores and sales
5. Statistical Hypothesis Testing (scipy.stats)
```

---

## 📊 Key Findings & Conclusions

### 🕹️ Platforms
- The **top 5 platforms by total sales** were identified, showing that legacy consoles like **Wii and NES** had blockbuster titles that sold exceptionally well.
- Platform lifespan analysis revealed that most platforms remain commercially active for **5–11 years** before declining.
- Data was filtered from **2000 to 2016** to ensure data quality and build a reliable model for 2017 projections.

### 📉 Scores vs. Sales
- **There is no strong correlation between user/critic scores and sales.** A game can receive a low score and still achieve high sales figures.
- Commercial success depends more on **genre, platform, and region** than on review scores.
- Most users **do not leave reviews**, which limits feedback for game developers and can affect product improvement cycles.

### 🌍 Regional Preferences
- **North America:** Prefers action and shooter genres on Xbox and PlayStation platforms.
- **Europe:** Similar preferences to NA, with strong performance on PS platforms.
- **Japan:** Distinctly different — favors role-playing games (RPGs) and handheld platforms like the DS.
- **ESRB ratings** show that **M-rated (Mature)** games dominate NA and EU sales, while Japan's market is less influenced by ESRB classifications.

### 🧪 Statistical Hypothesis Testing
- **Xbox One vs. PC user ratings:** The p-value from Levene's test was above 0.05, meaning we **fail to reject the null hypothesis** — there is no statistically significant difference between average ratings on both platforms.
- **Action vs. Sports genre ratings:** With a p-value of 0.1148 (> 0.05), we **fail to reject the null hypothesis** — the average user ratings for Action and Sports games are not statistically different.


---

## 📁 Project Structure

```
📦 video-game-sales-analysis
 ┣ 📓 Video_game_Analysis.ipynb   # Main notebook with full analysis
 ┗ 📄 README.md
```

---

---

⭐ *If you found this project useful, feel free to leave a star!*
