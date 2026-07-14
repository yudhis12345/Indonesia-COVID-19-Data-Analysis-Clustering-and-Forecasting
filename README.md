# Indonesia COVID-19 Data Analysis, Clustering, and Forecasting

A data analysis and machine learning project focused on exploring the impact and patterns of COVID-19 across provinces in Indonesia. This project includes exploratory data analysis, province clustering using DBSCAN and K-Means, and time series forecasting of COVID-19 cases using a Multi-Layer Perceptron (MLP).

## Project Objectives

- Explore COVID-19 trends and patterns across Indonesia.
- Analyze relationships between demographic characteristics and the impact of COVID-19.
- Identify provinces with similar COVID-19 and demographic characteristics.
- Compare clustering approaches using DBSCAN and K-Means.
- Forecast COVID-19 cases using a Multi-Layer Perceptron (MLP) model.

## Dataset

The project uses the **COVID-19 Indonesia Dataset**, which contains time-series data at both national and provincial levels.

The dataset includes information such as:

- Daily and total COVID-19 cases
- Deaths and recoveries
- Active cases
- Population density
- Province and island information
- Number of cities and regencies
- Demographic and geographic information

## Project Workflow

### 1. Data Acquisition and Understanding

The dataset is loaded and explored to understand:

- Dataset dimensions
- Data types
- Missing values
- Available features
- National and provincial-level records

### 2. Data Cleaning

The data cleaning process includes:

- Handling missing values
- Correcting negative values in COVID-19 case-related columns
- Preparing national and provincial datasets
- Selecting relevant features for analysis and modeling

### 3. Exploratory Data Analysis

Exploratory Data Analysis (EDA) is performed to understand COVID-19 patterns in Indonesia.

The analysis includes:

- Correlation analysis between COVID-19 and demographic variables
- Identification of provinces with high COVID-19 mortality rates
- Analysis of population density and COVID-19 mortality
- Visualization of national COVID-19 trends over time

## Machine Learning Methods

### DBSCAN Clustering

DBSCAN is used to group provinces based on similarities in COVID-19 impact and demographic characteristics.

Features used include:

- Total Cases per Million
- Total Deaths per Million
- Population Density
- Total Cities

A parameter search is performed to evaluate different combinations of `eps` and `min_samples`.

### K-Means Clustering

K-Means is used as another clustering approach to segment provinces based on similar characteristics.

The optimal number of clusters is evaluated using the **Silhouette Score**.

### MLP Time Series Forecasting

A Multi-Layer Perceptron (MLP) model is used to forecast COVID-19 cases based on historical case data.

Lag features are created from previous observations:

- 1-day lag
- 7-day lag
- 14-day lag
- 30-day lag

The data is divided chronologically into training and testing sets to preserve the time-series structure.

## Technologies and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Machine Learning Techniques

- Exploratory Data Analysis (EDA)
- Data Preprocessing
- Feature Scaling
- DBSCAN Clustering
- K-Means Clustering
- Silhouette Score Evaluation
- Multi-Layer Perceptron (MLP)
- Time Series Forecasting
- Lag Feature Engineering

## Project Structure

```text
Indonesia-COVID19-Data-Analysis/
│
├── Covid_19_UAS_PVD.ipynb
├── covid_19_indonesia_time_series_all.csv
└── README.md
```

## How to Run

1. Clone or download this repository.

2. Install the required Python libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

3. Open the Jupyter Notebook:

```bash
jupyter notebook Covid_19_UAS_PVD.ipynb
```

4. Run the notebook cells sequentially.

## Authors

- Aiko Putri Pertama Lee
- Yudhistira
- Hsie Aiko Sachi

Data Science & Analytics  
Petra Christian University
