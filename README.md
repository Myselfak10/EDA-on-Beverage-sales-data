# EDA on Beverage Sales Data

This repository hosts an exploratory data analysis (EDA) project on a synthetic beverage sales dataset using Python. The project demonstrates data cleaning, correlation analysis, visualization, and machine learning to extract valuable insights from the data. [1] [2]

## Table of Contents

- [Introduction](#introduction)
- [Dataset Description](#dataset-description)
- [Installation](#installation)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
  - [Data Cleaning and Processing](#data-cleaning-and-processing)
  - [Correlation Analysis](#correlation-analysis)
  - [Visualizations](#visualizations)
- [Machine Learning Analysis](#machine-learning-analysis)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [License](#license)
- [Contact](#contact)
- [Acknowledgements](#acknowledgements)

## Introduction

This project performs an extensive exploratory data analysis on a synthetic beverage sales dataset using popular Python libraries. The analysis covers data integrity checks, grouping, correlations, and visualization of key metrics, as well as implementing a machine learning model to evaluate feature importance. [1] [2]

## Dataset Description

The dataset contains 8,999,910 rows and 11 columns with the following key fields:
- **Order_ID**
- **Customer_ID**
- **Customer_Type** (B2B, B2C)
- **Product**
- **Category**
- **Unit_Price**
- **Quantity**
- **Discount**
- **Total_Price**
- **Region**
- **Order_Date**

All columns were verified to have no null values or duplicates. [1] [2]

## Installation

Ensure you have Python 3.x installed on your machine. Then install the required packages using pip:


These libraries are used for data manipulation, visualization, and machine learning. [1] [2]

## Exploratory Data Analysis (EDA)

### Data Cleaning and Processing

- The dataset is loaded into a Pandas DataFrame from a CSV file.
- Checks for null values and duplicate entries confirmed data integrity.
- A validation step ensures that numeric columns (e.g., `Discount`) do not contain non-numeric values. [1] [2]

### Correlation Analysis

- A correlation matrix is computed for features such as `Unit_Price`, `Quantity`, `Discount`, and `Total_Price`.
- A Seaborn heatmap is constructed to visualize correlations, revealing noteworthy relationships between product price and total sales. [1] [2]

### Visualizations

- **Bar Graphs:** Grouping by `Category` and `Product` allows the identification of the most popular products measured by quantity sold.
- **Pie Charts:** These are employed to display the share of B2B and B2C customers as well as to illustrate the proportion of total sales captured by top products and categories.
- Additional grouping and aggregation computations help identify key revenue contributions. [1] [2]

## Machine Learning Analysis

A RandomForestClassifier is used to further analyze the data:
- The model is trained to classify data and returns perfect accuracy on both training and test splits (with a note that this may be due to the synthetic nature of the dataset). [1] [2]
- Feature importance is computed, highlighting that `Discount` and `Quantity` have the most significant impact on predictions. [1] [2]

## Project Structure


This structure separates the raw data, analysis notebooks, and supporting documentation. [1] [2]

## Usage

1. **Clone the repository:**
[1] [2]
2. **Install the dependencies** as described in the Installation section.
3. **Open the Jupyter Notebook** `EDA_on_Beverage_Sales_Data.ipynb` located in the `notebooks/` folder.
4. **Run the notebook cells sequentially** to perform data cleaning, generate visualizations, and evaluate the machine learning model. [1] [2]

## License

This project is licensed under the [MIT License](LICENSE). [1] [2]

## Contact

For any questions or feedback, please contact:  
- **Your Name** – [your.email@example.com](mailto:your.email@example.com)  
- GitHub: [https://github.com/yourusername](https://github.com/yourusername) [1] [2]

## Acknowledgements

- Many thanks to the developers behind Pandas, Seaborn, Matplotlib, and scikit-learn for their invaluable open-source tools. [1] [2]
- Appreciation is also extended to the community resources that provided guidance and best practices for conducting EDA and implementing machine learning. [1] [2]
