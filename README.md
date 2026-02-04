# CA01 – Exploratory Data Analysis: House Price Dataset

## Project Overview
This project performs Exploratory Data Analysis (EDA) on the Ames Housing dataset
to understand data structure, identify quality issues, and prepare the data
for future machine learning modeling. The goal is to make the dataset
"analytics-ready" by applying systematic data understanding and cleaning steps.

## Dataset
- **Source:** Ames Housing Dataset
- **File Used:** house-price-train.csv
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
- Data Quality Report identifying missing values and outliers

### Part 2: Data Cleaning
- Handling missing values using domain-aware strategies
- Removing extreme outliers conservatively
- Preparing clean numerical and categorical features

### Part 3: Collinearity & Feature Selection
- Correlation heatmap visualization
- Identification of highly correlated features
- Feature selection recommendations (no modeling performed)

## Notes
- No machine learning model is built in this assignment
- Encoding and scaling are deferred, as the focus is EDA
- All explanations, observations, and conclusions are included in the notebook

## Acknowledgements
Dataset provided by Ames Housing and course materials from MSBA CA01.

