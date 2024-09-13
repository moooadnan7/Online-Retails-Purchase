# Online-Retails-Purchase
in this notebook I practice the analysis and visualization of data using (pandas , numpy , matplotlib , plotly , seaborn)
# steps
Step 1: Import Libraries

Import the necessary libraries for data manipulation and visualization.
Example: import pandas as pd and import matplotlib.pyplot as plt
Step 2: Import the Dataset

Import the dataset from the specified address.
Example: online_rt = pd.read_csv('dataset_address.csv', encoding='latin1')
Step 3: Prepare Data

Assign the dataset to a variable called online_rt.
Note: If you receive a UTF-8 decode error, set encoding='latin1' in pd.read_csv().
Step 4: Create a Histogram

Create a histogram for the 10 countries with the highest 'Quantity' ordered, excluding the UK.
Step 5: Filter Data

Exclude entries with negative 'Quantity' values.
Step 6: Create a Scatterplot

Generate a scatterplot with 'Quantity' versus 'UnitPrice' by 'CustomerID' for the top 3 countries (excluding the UK).
Step 7: Investigate Results

Analyze why the scatterplot might look uninformative.

Step 7.1: Examine Code and Data

Look at the first line of code in Step 6 and determine if it might lead to issues.

Step 7.1.1: Display Data

Display the first few rows of the DataFrame.
Step 7.1.2: Check Data Types

Display the data type of 'UnitPrice'.
Step 7.1.3: Filter Customer Data

Extract data for CustomerIDs 12346.0 and 12347.0.
Step 7.2: Reinterpret the Problem

Reassess the problem statement: "Create a scatterplot with the Quantity per UnitPrice by CustomerID for the top 3 Countries".

Step 7.2.1: Identify Top 3 Countries

Find the top 3 countries based on total sales volume (i.e., total quantity sold).
Step 7.2.2: Define Plot Requirements

For 'Quantity per UnitPrice by CustomerID', decide how to represent:
Quantity per customer (total Quantity)
Average UnitPrice per customer
Step 7.3: Modify and Plot Data

Step 7.3.1: Calculate Revenue

Add a 'Revenue' column to online_rt by calculating Quantity * UnitPrice.
Step 7.3.2: Compute Average Price

Group by 'CustomerID' and 'Country' to find the average price per unit.
Step 7.3.3: Plot Data

Plot the scatterplot with updated data.
Step 7.4: Broaden Analysis

Consider plotting data without country restrictions to see overall trends.

Step 7.4.1: Plot All Data

Plot the data for each 'CustomerID' on a single graph.
Step 7.4.2: Zoom In

Zoom in on the graph to better observe trends.
Step 8: Analyze Revenue vs. UnitPrice

Plot a line chart showing 'Revenue' (y) per 'UnitPrice' (x).

Step 8.1: Group Data

Group 'UnitPrice' into intervals of 1 for prices [0,50) and sum 'Quantity' and 'Revenue'.
