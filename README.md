# stockholm_lp1_colla_project_sprint_1

 stockholm collaborative project on Regression models

Here is the detailed data cleaning process based on the provided information in data sets

1. Installing Packages:

Install the matplotlib package using %pip install matplotlib.
Install the seaborn package using %pip install seaborn.
2. Importing Packages:

Import the required packages: pandas, numpy, matplotlib.pyplot, and seaborn.
Use the following import statements:
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
3. Read Data:

Read the 'startup_funding2018.csv' file and convert it to a pandas DataFrame using pd.read_csv('startup_funding2018.csv').
Assign it to the variable df.
Read Data:

Read the 'startup_funding2019.csv' file and convert it to a pandas DataFrame using pd.read_csv('startup_funding2019.csv').
Assign it to the variable df2.
4. View Data:

Use df.head() to view the first few rows of the DataFrame df.
Use df2.head() to view the first few rows of the DataFrame df2.
5. Get Information:

Use df.info() to get information about the DataFrame df.
Use df2.info() to get information about the DataFrame df2.
6. Descriptive Statistics:

Use df.describe(include='object') to generate descriptive statistics of the DataFrame df.
Use df2.describe(include='object') to generate descriptive statistics of the DataFrame df2.
7. Missing Values:

Use missing_values = df.isnull().sum() to calculate the number of missing values in each column of df.
Print missing_values to see the results.
Use missing_values2 = df2.isnull().sum() to calculate the number of missing values in each column of df2.
Print missing_values2 to see the results
8. Replace Specific Values with NaN:

Use df2['Founded'].replace('Unknown', np.nan, inplace=True) to replace 'Unknown' values in the 'Founded' column of df2 with NaN.
Use df2['HeadQuarter'].replace('Not available', np.nan, inplace=True) to replace 'Not available' values in the 'HeadQuarter' column of df2 with NaN.
Use df2['Sector'].replace('', np.nan, inplace=True) to replace empty string values in the 'Sector' column of df2 with NaN.
Use df2['Founders'].replace('', np.nan, inplace=True) to replace empty string values in the 'Founders' column of df2 with NaN.
Use df2['Stage'].replace('', np.nan, inplace=True) to replace empty string values in the 'Stage' column of df2 with NaN.
9. Check for Specific Symbols in data set one named as df:

Create a list columns_to_check containing the columns to check for the '-' symbol in df.
Iterate over the columns in columns_to_check using a for loop.
Use has_dash_symbols = df[column].str.contains('—').any() to check if the column contains the '-' symbol.
Print the result using print(f"{column}: {has_dash_symbols}").
10.Check for Specific Symbols in data frame 2 named as df2:

Create a list columns_to_check2 containing the columns to check for the '-' symbol in df2.
