# Fortnite Player Performance Insights

## Description
This project demonstrates data cleaning, transformation, and analysis of Fortnite performance statistics derived from Kaggle using Python and pandas.  
It covers handling missing values, standardising column names, deriving new metrics, categorising players, and aggregating data for insights. Engineered custom metrics to categorise players and revealed trends in eliminations, accuracy, and behavioural factors.

**Key Features:**
- **Data cleaning:** loaded CSV with pandas, standardised and renamed columns, handled missing values, duplicates, and impossible values; previewing data with 'head()'.
- **Feature Engineering:** calculated headshot accuracy (%) and defined elimination categories (Low / Medium / High); grouping with 'groupby()'.
- **Data aggregation:** computed averages and proportions, minimum and maximum values to explore player performance.  
- **Insights & limitations:** examined relationships between eliminations, accuracy, time of day, and reported mental state; highlighted data constraints, recommendations and potential reasons for findings.
- **Export:** cleaned dataset saved for data visualisation.

## Dataset
- Each row represents a Fortnite game session.  
- Columns include:
  - `date`: Date of the match  
  - `time of day`: Match start time  
  - `placed`: Placement in match  
  - `mental state`: Player condition (e.g., sober, high)  
  - `eliminations`: Number of kills  
  - `assists`, `revives`  
  - `accuracy`, `hits`, `head shots`  
  - `distance traveled`  
  - `materials gathered`, `materials used`  
  - `damage taken`, `damage to players`, `damage to structures`  
  - `headshot_accuracy`: Calculated as `(head shots / hits) * 100`  
  - `elimination_category`: Categorized as Low, Medium, High  

## How to Use
1. Clone or download the repository  
2. Place the dataset `Performance_Statistics.csv` in the working directory  
3. Open `fortnite_analysis.py` (or run in Jupyter Notebook)  
4. Execute the script sequentially to:
   - Inspect and clean the data  
   - Derive new metrics and categorize players  
   - Generate aggregated statistics  
5. The cleaned dataset will be exported as `fortnite_cleaned_project.csv`  

## Notes
- Eliminations are categorized into Low (<=2), Medium (3–5), and High (>5)  
- Aggregated statistics include averages by time of day and mental state  
- This project illustrates practical data cleaning and exploratory data analysis for gaming datasets
