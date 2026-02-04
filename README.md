# CA01 – Exploratory Data Analysis: House Price Dataset

## Project Overview
This project performs Exploratory Data Analysis (EDA) on the Ames Housing dataset to
understand the data structure, identify data quality issues, and prepare the dataset
for future machine learning modeling. The goal is to make the data analytics-ready
through systematic data understanding and cleaning, without performing model training.

## Dataset
- **Source:** Ames Housing Training Dataset (provided via course GitHub repository)  
  https://github.com/ArinB/MSBA-CA-Data/raw/main/CA01/house-price-train.csv
- **Target Variable:** SalePrice
- **Description File:** data_description.txt

## Project Structure
- `CA01_EDA_House_Price.ipynb` – Main notebook containing all analysis
- `house-price-train.csv` – Training dataset
- `data_description.txt` – Feature definitions and domain information
- `README.md` – Project documentation

## Environment & Libraries
The following Python libraries are required:
- pandas
- numpy
- matplotlib
- seaborn

Python version: 3.x  
Notebook environment: Jupyter / Google Colab

## Analysis Workflow
The notebook follows the three required CA01 stages:

### Part 1: Data Understanding
- Dataset structure and data types
- Summary statistics
- Univariate and bivariate visualizations
- Data Quality Report identifying missing values and potential outliers

### Part 2: Data Cleaning
- Handling missing values using domain-aware strategies
- Assessing and handling extreme outliers conservatively
- Preparing clean numerical and categorical features

### Part 3: Collinearity & Feature Selection
- Correlation heatmap visualization
- Identification of highly correlated features
- Feature selection recommendations (no modeling performed)

## Notes
- No machine learning model is built in this assignment
- Encoding and scaling are deferred, as the focus is EDA and data quality assessment
- All explanations, observations, and conclusions are included in the notebook

## Acknowledgements
Dataset and course materials provided by Dr. Arin Brahma for BSAN 6070.


