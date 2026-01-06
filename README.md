# 🎮 Video Game Industry: Identifying Success Patterns for Market Strategy

## 🎯 Project Overview
Working as a Data Analyst for the online store "Ice," this project focuses on identifying the variables that determine a video game's success. By analyzing historical data on sales, critic/user reviews, and platforms, the goal was to pinpoint "big winners" and plan a data-driven advertising campaign for 2017.

## 🛠️ Data Engineering & Wrangling
The dataset required significant preprocessing to ensure analytical integrity across multiple regions (NA, EU, JP):
* **Standardization:** Converted all column names to `snake_case`.
* **Type Conversion:** Handled the `TBD` (To Be Determined) values in user scores by treating them as nulls to allow for numerical calculation.
* **Feature Engineering:** Created a `total_sales` metric by aggregating revenue across all global regions.
* **Integrity Management:** Investigated and resolved missing values in release years and ESRB ratings to minimize bias in temporal analysis.


## 📊 Strategic Market Analysis

### 1. Platform Lifecycle & Transition
I analyzed the rise and fall of gaming platforms (Xbox, PlayStation, PC, etc.), identifying that platforms typically have a **10-year lifecycle**, with a 5-year peak. This allowed for the identification of "dying" vs. "emerging" platforms for the 2017 budget.

### 2. Regional User Profiling
A key part of the project involved creating distinct profiles for different markets:
* **North America & Europe:** Driven by Action/Shooter genres and mature ESRB ratings.
* **Japan:** Highly influenced by Role-Playing (RPG) games and handheld platforms.

### 3. Review Impact Analysis
Using scatter plots and correlation matrices, I evaluated how much professional critic scores vs. user reviews actually drive sales performance.

## 🧪 Statistical Hypothesis Testing
Two independent sample **t-tests** were conducted with a significance level ($\alpha$) of **0.05**:
1.  **Platform Comparison:** Testing if the average user ratings for **Xbox One** and **PC** differ.
2.  **Genre Comparison:** Testing if average user ratings for **Action** and **Sports** genres are distinct.

## 🛠️ Tech Stack
* **Language:** Python 3.12.1
* **Analysis:** Pandas, NumPy.
* **Visualization:** Matplotlib, Seaborn (Boxplots, Scatter plots, Area charts).
* **Statistics:** SciPy.

## 📈 Final Conclusions
The analysis successfully identified that while global sales are concentrated in high-performance consoles, Japan requires a specialized marketing approach. For 2017, the recommendation focuses on prioritizing emerging platforms mid-way through their lifecycle and tailoring genre-specific ads based on regional preferences.
