# Data601Assignment4
City of Calgary Building Energy Benchmarketing Dataset Visualization

### Overview
This repository performs an in-depth analysis on the City of Calgary's Building Energy Bencharmarking dataset. Using python and a number of libraries such as pandas, numpy, matplotlib and seaborn, the analysis involves cleaning the data, exploration, visualization of key trends and statistical testing to extract valuable insights into energy consumption patterns and emissions. 

### Structure
The reposity contains the following components:
- Jupyter Notebook: contains all the python code for the entire analysis
- Report: Summarizes Key findings, trends and insights from the python analysis
- Folder Structure:
  - data/
  - notebook/
  - report/

### Methodology
1. Data Cleaning
  - Handling missing values
    - Columns with over 40% missing values were dropped
    - Numerical missing values were replaced by the median with respect to the column
    - Categorical missing values were replaced by the mode with respect to the column
  - **Regex Usage**
    - Extracted numerical values from columns containing units in brackets (Ex. Total GHG Emissions (Metric Tons CO2e)
    - Standardized postal codes to follow Canadian format (Ex. A1A 1A1)
    - Cleaned property names and addresses by removing special characters
2. Exploratory Data Analysis
  - Generated Statistical Summary
  - Aggregated Data based on specific groupings
  - **Regex Usage**
    - Identified values not conforming to expected numerical formats
    - Removed values that did not follow the expected formats
  - Applied IQR methods to detect outliers in the data
3. Visualizations
  - Yearly Trend Time Series Analysis
  - Bar Chart
  - Heatmap
4. Statistical Testing
  - Correlation Analysis
  - Hypothesis Testing

### Challenges Faced
- Visualization Clarity
  - Managing overlapping x-axis labels for property names
- Effective Grouping
  - Had to ensure effective grouping in python by columns, especially for visualizations and data exploration
- Regex
  - Implementing effective Regex was the biggest challenge, learning the library and making sure the code was effective took a lot of time and effort
