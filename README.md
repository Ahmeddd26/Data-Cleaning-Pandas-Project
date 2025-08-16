Data Cleaning Project: Pakistan Drone Attacks Dataset
This project focuses on the end-to-end process of cleaning and preparing the "Pakistan Drone Attacks" dataset. Starting with the raw source file, this project demonstrates a comprehensive data wrangling workflow using the Pandas library in Python to transform the data into a clean, structured, and analysis-ready format.

Dataset
The dataset contains information about drone strikes in Pakistan, including details on location, casualties, and other associated data. The primary challenge was to clean this data to make it reliable for future exploratory data analysis and visualization.

Tools and Libraries
Python 3.9

Pandas

Jupyter Notebook (run in Visual Studio Code)

Data Cleaning and Preparation Workflow
The following steps were performed to clean and prepare the data:

Data Loading and Initial Inspection:

Loaded the raw CSV file into a Pandas DataFrame.

Overcame initial challenges including file path issues, UnicodeDecodeError by specifying the correct encoding, and various SyntaxErrors during debugging.

Column Renaming:

Renamed columns for better clarity and easier access during analysis (e.g., 'Women/Children' was renamed to 'Deaths').

Handling Missing Values:

Identified numerical columns containing missing values (NaN).

Filled these missing values with 0 to ensure the columns could be used for mathematical operations and calculations.

Correcting Data Types:

Used the .astype() method to convert columns to their appropriate data types. For example, columns intended for numerical analysis were converted from object to int or the nullable Int64 type.

Exploratory Analysis & Verification:

Performed basic grouping and aggregation using .groupby() to understand the data's structure (e.g., calculating totals per province).

Used .value_counts() on categorical columns like 'City' to check the frequency of occurrences.

Saving the Cleaned Data:

Exported the final, clean DataFrame to a new CSV file (Cleaned Drone Attack.csv) with the index excluded, making it ready for future use.

Repository Structure
├── Drone Attacks.ipynb         # The main Jupyter Notebook with all the cleaning steps and code.
├── original_dataset.csv        # The raw, unprocessed dataset used as the starting point.
└── Cleaned Drone Attack.csv    # The final, clean, and structured dataset produced by t
