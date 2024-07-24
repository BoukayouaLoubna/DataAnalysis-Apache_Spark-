# DataAnalysis-Apache_Spark-

## Project Overview:

The project aims to analyze IPL (Indian Premier League) cricket data using PySpark and visualize various statistics and insights.  
The primary objectives include data preprocessing, feature engineering, and performing different analyses to uncover interesting patterns and trends in the IPL matches.  

## Archetecture:  

## Workflow : 

### 1. Importing Necessary Libraries:  
Initializes a Spark session to work with Spark DataFrames and perform large-scale data processing.

### 2. Define Schemas:
- Defines schemas for different datasets including ball-by-ball data, match data, player data, player match data, and team data.
- This ensures structured data processing with predefined data types for each column.
  
### 3. Data Preparation and Feature Engineering:
- Filters valid deliveries (excluding wides and no balls).
- Aggregates runs to calculate total and average runs per match and inning.
- Computes cumulative runs for each over within each match.
- Flags high-impact deliveries (either a wicket or more than 6 runs).
  
### 4. Feature Engineering for Match Data Analysis:
- Extracts temporal features (year, month, day) from match dates.
- Categorizes win margins into 'High' or 'Low'.
- Calculates total wins per team and season.
- Determines team performance based on batting/bowling order and toss outcomes.
  
### 5. Data Exploration and Analysis:
Using Various SQL queries and DataFrame operations  to derive insights, such as:  
- Most frequent venues.
- Distribution of match outcomes.
- Top-performing teams, players, and overall statistics.
  
### 6. Data Visualization:
Several visualizations are created using Matplotlib and Seaborn to present the analyzed data:  
- a. Team Performance by Season:
Shows the number of wins for each team per season using a bar plot.

- b. Home vs Away Performance:
Compares the number of home and away wins for each team using a dual-colored bar plot.

- c. Most Economical Bowlers in Powerplay Overs:
Displays the top 10 economical bowlers in powerplay overs.

- d. Impact of Winning Toss on Match Outcomes:
Shows the count of matches won or lost after winning the toss using a count plot.

- e. Top Batsmen Based on Total Runs Scored:
Lists the top 10 batsmen with the highest total runs.

- f. Top Bowlers Based on Wickets Taken:
Lists the top 10 bowlers with the highest number of wickets.

- g. Average Runs Scored Per Over:
Displays the average runs scored per over.

- h. Teams' Performance by Season:
Shows the number of wins by each team per season.

- I. Home vs Away Performance:
Compares home and away wins for each team.

## Tools:  
- AWS S3: For storing and retrieving large datasets.
- Databricks: For collaborative data science and big data analytics.
- PySpark: For large-scale data processing and manipulation.
- Pandas: For converting Spark DataFrames to Pandas DataFrames for easier manipulation and plotting.
- Matplotlib: For creating various static, interactive, and animated visualizations.
- Seaborn: For statistical data visualization, making it easier to create attractive and informative statistical graphics.
- SQL: Embedded within PySpark for querying data directly from Spark DataFrames.

## Conclusion:  
This project leverages Spark's processing power and visualization capabilities of diffrent Tools to analyze and present insights from the IPL dataset effectively.
