
# Data Analysis Project: Zomato Dataset

## Project Description
This project involves an in-depth exploratory data analysis (EDA) of a Zomato restaurant dataset. The goal is to uncover insights related to restaurant ratings, cuisine preferences, cost distribution, and the impact of online ordering.

## Analysis Steps & Key Findings

### 1. Data Loading and Initial Inspection
- Loaded the `zomato.csv` dataset.
- Performed initial data inspections (`.head()`, `.info()`, `.isnull().sum()`).

### 2. Data Cleaning and Preprocessing
- Dropped irrelevant columns (`url`, `phone`, `address`, `menu_item`, `reviews_list`).
- Cleaned and converted `rate` column to numeric, filling missing values with the mode.
- Cleaned and converted `approx_cost(for two people)` to numeric, filling missing values with the median.
- Filled missing values in `location`, `rest_type`, `cuisines`, and `rating` with their respective modes.
- Filled missing values in `dish_liked` with 'Not Specified'.

### 3. Exploratory Data Analysis (EDA)
- **Distribution of Restaurant Rates**: Visualized the frequency of different restaurant ratings.
- **Distribution of Approximate Cost for Two People**: Analyzed the spread of dining costs.
- **Distribution of Votes**: Explored the number of votes received by restaurants.
- **Relationship between Rate and Online Order Availability**: Examined how online order options affect ratings using a violin plot.
- **Top 15 Cuisines Rate Distribution**: Visualized the rate distribution for the most popular cuisines.

### 4. Characteristics of Highest-Rated Restaurants (Rate 4.9)
- Identified restaurants with the maximum rate (4.9).
- Analyzed common **cuisines**: 'Asian', 'North Indian', 'Momos', 'Thai', 'Chinese' were prominent.
- Analyzed common **locations**: 'Koramangala 5th Block', 'Brigade Road', 'BTM' were frequently observed.
- Analyzed **approximate cost**: Mean cost of ~1274.55 INR, indicating a mid-to-high budget segment.

### 5. Comparison: Highest-Rated vs. Average-Rated Cuisines
- Defined average-rated restaurants as those with a rate between 3.5 and 4.0.
- Compared top 10 cuisines for both highest-rated and average-rated restaurants.
- **Key Findings**:
    - **Shared Popularity**: 'North Indian', 'Chinese', 'Desserts', 'Continental' are popular across both categories.
    - **Highest-Rated Differentiators**: Cuisines like 'Asian', 'Momos', 'Thai', 'Mediterranean', 'BBQ', 'European' are more prominent in the highest-rated group, suggesting specialization or exceptional execution.
    - **Average-Rated Volume**: 'South Indian', 'Fast Food', 'Biryani', 'Beverages', 'Cafe', 'Bakery' are highly frequent in the average-rated group, catering to broad, everyday demand.
    - **Quality vs. Volume**: Significant scale difference; achieving highest ratings with common cuisines is rare, indicating superior quality.

## Visualizations and Reports
All generated plots and analysis reports (if applicable) are saved in the `analysis_reports/` directory within this project. You can find detailed figures such as:
- `distribution_of_restaurant_rates.pdf`
- `distribution_of_approx_cost.pdf`
- `distribution_of_votes.pdf`
- `rate_by_online_order.pdf`
- `top_cuisines_comparison.pdf` and etc

## Project Structure
```
ds_Sangeetha/
├── csv_files/
├── outputs/
├── zomato.ipynb
├── README.md
```

## How to Use
1.  **Clone this repository** (if applicable).
2.  **Open the Jupyter Notebooks** (`notebook_1.ipynb`, `notebook_2.ipynb`) to follow the analysis steps.
3.  **Inspect the `analysis_reports/` folder** for all generated visualizations and PDF reports.

