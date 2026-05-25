# Video Game Retail Analysis — Global Market Trends & Consumer Behavior
## 📌 Project Overview

This project analyzes global video game sales data to identify market trends, platform performance, genre profitability, and regional consumer preferences across North America, Europe, and Japan.

The analysis focuses on understanding how different factors — such as platform popularity, genre, ESRB rating, and review scores — influence commercial success in the gaming industry.

## 🎯 Objective

The main goal of this project was to discover meaningful business insights from historical video game sales data and evaluate:

Which platforms generate the highest sales
Which genres are the most profitable globally
How user and critic reviews affect sales performance
How gaming preferences differ between regions
Whether statistical differences exist between user ratings of different platforms and genres

## 📂 Dataset
Dataset name: games.csv
Total records: 16,715 rows
Original features (11):
Name
Platform
Year_of_Release
Genre
NA_sales
EU_sales
JP_sales
Other_sales
Critic_Score
User_Score
Rating
Created Feature

total_sales

Calculated as:
NA_sales + EU_sales + JP_sales
🛠️ Tools & Libraries Used

The project was developed using Python and the following libraries:

pandas
numpy
matplotlib
seaborn
scipy.stats
math

## 🧹 Data Cleaning & Preprocessing

Several preprocessing steps were performed to improve consistency and analysis quality:

Renamed all column names to lowercase
Converted year_of_release from float to Int64

Converted user_score from object to float

"TBD" values were transformed into NaN using:
errors='coerce'
Checked and confirmed there were no duplicated rows
Missing values were intentionally preserved to maintain data integrity
Filtered the dataset to include only games released from 2014 onward for modern market relevance


## 🔍 Methodology

The analysis was performed through the following steps:

Exploratory Data Analysis (EDA)
Release trends over time
Platform performance
Genre profitability
Regional sales comparisons
Data Visualization
Bar charts
Scatterplots
Correlation analysis
Boxplots for sales distribution
Statistical Analysis
Hypothesis testing using independent t-tests
Comparison of user review averages between platforms and genres


## 📊 KPIs & Key Findings
🎮 Game Releases by Year
Video game releases peaked between 2008 and 2009
Approximately 1,400 games were launched annually during this period
🕹️ Best-Selling Platforms
Historical Overall Leader
PS2 generated the highest total sales historically
Leading Platforms Since 2014
PS4
Xbox One
Nintendo 3DS

These platforms dominated the modern market analysis period.

### 📈 Sales Distribution by Platform

Boxplot analysis showed that:

PS4
Xbox One
Wii

had the largest sales dispersion, indicating the presence of major blockbuster titles.

### ⭐ Review Scores vs Sales
Critic Scores
Moderate positive correlation with sales:
Correlation ≈ 0.40
User Scores
Almost no meaningful correlation with sales:
Correlation ≈ -0.04
Insight

Professional critic reviews appear to influence purchasing behavior more strongly than user reviews.

### 🎯 Genre Performance

Top-performing genres globally:

Action → ~176M sales
Shooter → ~149M sales

These genres consistently showed the highest commercial performance.

### 🌍 Regional Preferences
North America & Europe
Strong preference for:
Action games
Shooter games
ESRB rating M (Mature)
Japan
Strong preference for:
RPG games
Portable gaming platforms (especially 3DS)

### 🧪 Hypothesis Testing
#### 1️⃣ Xbox One vs PC User Scores
Hypotheses
H₀: Average user scores are equal
H₁: Average user scores are different
Result
p-value = 0.116
Conclusion

The null hypothesis could not be rejected.
There is no statistically significant difference between Xbox One and PC user scores.

#### 2️⃣ Action vs Sports User Scores
Hypotheses
H₀: Average user scores are equal
H₁: Average user scores are different
Result
p-value = 1.18e-14
Conclusion

The null hypothesis was rejected.
Action games received statistically different (and generally higher) user scores than Sports games.

## 📌 Final Conclusions
PS4 dominated Western markets, while Nintendo 3DS remained highly successful in Japan
Action and Shooter games generated the highest profitability worldwide
Regional preferences strongly influence platform and genre success
Critic reviews impact sales more than user reviews
Genre has a stronger effect on user perception than platform choice
## ▶️ How to Run the Project
Requirements

Install the required Python libraries:

pip install pandas numpy matplotlib seaborn scipy
Run the Notebook

Open the Jupyter Notebook or Google Colab file and execute the cells sequentially.

📁 Project Structure
├── games.csv
├── video_game_analysis.ipynb
└── README.md
📬 Author

## Data Analysis Project
### Created by Hugo Ardila