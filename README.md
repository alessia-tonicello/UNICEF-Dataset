# UNICEF Dataset
This project performs an exploratory data analysis (EDA) on the UNICEF dataset available at [UNICEF's website]. The analysis focuses on various indicators, such as GDP per capita, life expectancy, dependency ratios, and population statistics for different countries. Visualizations, including correlation heatmaps and bar plots, are used to highlight key insights and trends.

## Dataset
The dataset used for this project, _datasetunicef2.csv_, includes the features such as:
- Countries and regions
- Population (Total)
- GDP per capita
- Life expectancy at birth (2021)
- Dependency ratio (total)
- Dependency ratio (child)
- Dependency ratio (old age)

## Methodology
1. Data Loading and Exploration
   - Imported the dataset into a Pandas DataFrame.
     
2. Data Exploration and Cleaning
   - Missing Values: Identified missing values in the dataset and dropped rows with any missing data using the ```dropna()``` function.
   - Data Conversion: Converted the Population (Total) column to numeric format using ```pd.to_numeric()``` to ensure accurate analysis.

3. Data Analysis
   - Correlation Analysis: Computed the correlation matrix for numerical columns to identify relationships between variables like GDP, life expectancy, and population.
   - Country Comparisons:
      - Compared countries with GDP and life expectancy above and below the mean.
      - Identified the top 3 countries with the highest and lowest GDP per capita and life expectancy.
      - Calculated the difference from the mean for each of these countries.

3. Visualizations
- Heatmap: Created a heatmap to show correlations between key numerical variables, such as GDP per capita and life expectancy.
- Bar Plots:
      - Visualized the top 3 and bottom 3 countries by GDP and life expectancy with bar plots.
      - Displayed the differences from the mean for each country's GDP and life expectancy.
- Boxplot: Created a boxplot to compare the three types of dependency ratios: total, child, and old age.

## Code Usage
1. Install Python Libraries:
   - You only need Python installed with the pandas library. Install it with: --> ```pip install pandas```

2. Run the Script:
   - Use the following command in your terminal to execute the analysis: --> ```python unicef_eda.py```

3. View the Output:
   - The script will display histograms for feature distributions and scatter plots displaying geographic trends, population density, and the relationship between median income and housing prices.

## Output
The script will generate the following outputs:
- A correlation heatmap to show relationships between numerical variables.
- Bar plots displaying the top and bottom 3 countries by GDP and life expectancy.
- A boxplot comparing the dependency ratios.

## Technologies Used
- **Python**: For data manipulation and analysis.
- **Pandas**:: For data cleaning and manipulation.
- **Matplotlib**: For visualizations like bar plots and heatmaps.
- **Seaborn**: For advanced plotting, such as the correlation heatmap and boxplots.
- **Jupyter Notebook**: For an interactive environment to run and display code.




