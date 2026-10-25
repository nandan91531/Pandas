# Pandas Practice

A simple, hands-on project to learn **Pandas** with Python. This repository contains Jupyter notebooks that explain the main Pandas concepts with small examples and practice datasets.

## What is Pandas?

Pandas is a Python library used to work with data. It helps us read data from files, organize it into tables, clean missing values, filter rows, calculate summaries, and find useful information.

## What You Will Learn

- **Series:** Create and work with one-dimensional labeled data.
- **DataFrames:** Create tables, select rows and columns, add or remove columns, and filter data using conditions.
- **Missing Data:** Find missing values, remove rows with missing data, and fill missing values.
- **Merge, Join, and Concatenation:** Combine data from multiple DataFrames in different ways.
- **GroupBy and Aggregation:** Group data and calculate values such as sum, mean, minimum, maximum, count, and median.
- **Pivot Tables and Cross Tabs:** Summarize data by categories and compare values across groups.
- **Basic Operations:** Check the shape and columns of a DataFrame, inspect data, calculate statistics, and apply functions to columns.
- **Feature Extraction:** Extract useful information from text, convert values to numeric types, and answer questions using the Anime dataset.
- **Data Analysis Practice:** Explore country data and answer questions about population, capitals, regions, democracy scores, and political leaders.

## Project Structure

```text
Pandas-Practice/
├── 1)Series.ipynb
├── 2)DataFrames.ipynb
├── 3)MissingData.ipynb
├── 4)MergingJoiningConcatination.ipynb
├── 5)GroupByAggregation.ipynb
├── 6)PivotTables.ipynb
├── 7)Operations.ipynb
├── FeatureExtraction.ipynb
├── Countries.ipynb
├── anime.csv
├── Countries.csv
└── README.md
```

## Tools Used

- Python
- Pandas
- NumPy
- Jupyter Notebook
- CSV files for practice

## Getting Started

### 1. Clone the repository

```bash
git clone YOUR_REPOSITORY_URL
cd YOUR_REPOSITORY_FOLDER
```

Replace the example values with your actual GitHub repository URL and folder name.

### 2. Install the required libraries

```bash
pip install pandas numpy jupyter
```

### 3. Start Jupyter Notebook

```bash
jupyter notebook
```

Open a notebook and run the cells from top to bottom. Keep the CSV files in the same folder as the notebooks that use them, so `pd.read_csv()` can find the data.

## Practice Datasets

- **Countries.csv:** Used to explore country information, including population, capital cities, regions, democracy scores, and political leaders.
- **anime.csv:** Used to practice extracting information from anime titles, working with episode counts, and answering questions about scores and episodes.

## Example

Find the country with the highest population:

```python
import pandas as pd

df = pd.read_csv("Countries.csv")
most_populated_country = df[df["population"] == df["population"].max()]
print(most_populated_country["country"])
```

Find the anime with the highest episode count:

```python
df = pd.read_csv("anime.csv")
df[df["Episodes"] == df["Episodes"].max()]["Title"]
```

The second example assumes the `Episodes` column has already been created, as shown in `FeatureExtraction.ipynb`.

## Learning Goal

The goal of this project is to build a strong foundation in Pandas by practicing with code and real-looking datasets. Try changing the examples, testing different conditions, and answering your own questions with the data.

## Author

Created as a Pandas learning and practice project.
