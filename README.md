# BIG-DATA-ANALYSIS

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: PONMATHI PALMURUGAN

*INTERN ID": CT06XHX

*DOMAIN*: PYSPARK

*DURATION*: 6 WEEKS

*MENTOR":  NEELA SANTHOSH

**IPL 2025 Unsold Players Data Analysis**
**Overview**
This project analyzes IPL match data to identify top-performing batsmen and bowlers who went unsold in the IPL 2025 auction. The analysis is performed using Apache Spark (PySpark) within a Databricks environment.

**Features**
Batsman Statistics: Calculates total runs, balls faced, strike rate, and boundaries (fours & sixes) for each batsman.

Bowler Statistics: Computes wickets taken, economy rate, and runs conceded for each bowler.

Auction Analysis: Identifies players who went unsold in the IPL 2025 auction.

Data Transformation: Formats player names correctly using UDFs.

Top Performers Analysis: Lists the top unsold batsmen and bowlers based on performance metrics.

**Technologies Used**
Databricks: For cloud-based data processing.

Apache Spark (PySpark): For large-scale data processing and transformation.

Python: Used for data manipulation and analysis.


**Dataset**
The project uses three CSV datasets:

matches.csv - Contains match details.
deliveries.csv - Ball-by-ball delivery data.
ipl_2025_auction_players.csv - List of players and their auction status.

**Data Processing Steps**
Load Data: Reads CSV files into Spark DataFrames.

Compute Batting Stats:
Group by batsman to calculate runs, balls faced, strike rate, and boundaries.
Filter batsmen who have faced at least 50 balls.

Compute Bowling Stats:
Count valid wickets (excluding run outs) for each bowler.
Compute economy rate based on runs conceded and overs bowled.

Format Player Names:
Use UDFs to standardize player names.
Convert full names to initials-based format for consistency.

Identify Unsold Players:

Filter out players marked as "Unsold" in the auction dataset.

Join Data:
Merge unsold players with batting and bowling statistics.

Display Top Performers:
List top 10 unsold batsmen based on strike rate and boundaries.
List top 10 unsold bowlers based on wickets and economy rate.

How to Run
Upload the datasets (matches.csv, deliveries.csv, ipl_2025_auction_players.csv) to Databricks.
Run the provided Databricks notebook in a PySpark environment.

Use display() commands to visualize top performers.

**Results**
Identifies underrated players who performed well but went unsold in the auction.

Highlights top batsmen with high strike rates and boundary counts.

Lists top bowlers with good wicket-taking ability and economy rates.
Screenshot 2025-03-24 091603 Screenshot 2025-03-24 091638

![Image](https://github.com/user-attachments/assets/4ae34fd6-d0cd-4407-92a7-a6e17f685724)

![Image](https://github.com/user-attachments/assets/4f106ed3-308e-449a-a5f7-9d1e63a92b52)
