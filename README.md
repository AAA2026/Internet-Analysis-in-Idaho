# Regional Electricity & Internet Analysis in Idaho

## Project Overview

This project performs an in-depth analysis of broadband internet metrics and satellite radiance data across various counties within the state of Idaho. Utilizing a comprehensive dataset that combines information on broadband availability, usage statistics, internet speeds, and geographical radiance measurements, the analysis aims to explore potential relationships and patterns between these factors. The primary tool for this analysis is a Jupyter Notebook which guides through the processes of data loading, cleaning, filtering, exploration, and visualization.

## Data Source

The core data for this analysis is contained within the `Project_df.csv` file. This dataset aggregates multiple variables related to geographic locations within the United States, including Federal Information Processing Standards (FIPS) codes, county names (NAMELSAD), state identifiers, population figures, broadband availability percentages reported by the FCC, broadband usage rates, and specific location identifiers (quadkey). It also includes technical metrics such as average download speed (avg_d_kbps), average upload speed (avg_u_kbps), average latency (avg_lat_ms), number of tests conducted, and devices involved. Furthermore, the dataset incorporates geospatial information derived from shapefiles (geometry, county FIPS, etc.) and detailed satellite radiance statistics (mean, min, max, median, standard deviation, quartiles) for the year 2020. For the purpose of this specific analysis, the dataset is filtered to focus exclusively on entries pertaining to the state of Idaho.

## Project Files

The main components of this project are located within the `Data Analysis` directory:

*   `DataAnalysis_PRJ_FINAL_.ipynb`: This Jupyter Notebook contains the complete Python code used for the analysis. It details the steps involved, from importing necessary libraries and loading the data, through data cleaning and preparation (including filtering for Idaho and handling missing values or redundant columns), to performing exploratory data analysis, statistical tests, and generating visualizations.
*   `Project_df.csv`: The primary dataset used in the analysis, as described in the Data Source section.

## Dependencies

To execute the analysis presented in the Jupyter Notebook, a Python environment with the following core libraries installed is required:

*   pandas: For data manipulation and reading the CSV file.
*   numpy: For numerical operations.
*   matplotlib: For creating static, interactive, and animated visualizations.
*   seaborn: For making statistical graphics more attractive and informative.
*   geopandas: For working with geospatial data.
*   shapely: For manipulation and analysis of planar geometric objects.
*   scipy: For scientific and technical computing, including statistical functions.

These dependencies can typically be installed using pip:

```bash
pip install pandas numpy matplotlib seaborn geopandas shapely scipy
```

## Usage Instructions

To replicate or explore the analysis:

1.  Ensure you have a Python environment set up with Jupyter Notebook or JupyterLab and the required dependencies installed (see Dependencies section).
2.  Navigate to the `Data Analysis` directory containing the notebook and the CSV file.
3.  Launch Jupyter Notebook or JupyterLab.
4.  Open the `Project.ipynb` notebook.
5.  Execute the cells sequentially to perform the data loading, cleaning, analysis, and visualization steps.

The notebook is structured to guide the user through the entire workflow, starting with library imports and data loading, followed by extensive data cleaning and preparation specifically tailored for the Idaho subset, and concluding with analytical steps likely involving correlation analysis and visualization to understand the interplay between broadband access, usage, and environmental radiance data within Idaho.

