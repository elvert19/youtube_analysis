


# YouTube Channel Data Analysis

## Overview

This project performs an exploratory data analysis (EDA) and statistical evaluation of YouTube channel data. It processes raw dataset files to uncover insights regarding channel performance, including view counts, subscriber bases, and growth patterns across different channel categories.

## Features

* **Data Extraction & Loading**: Automatically handles ZIP file extraction and loads CSV data (e.g., `youtube_channel_info_v1.csv`).
* **Data Cleaning**:
* Identifies and handles missing values.
* Converts temporal data (e.g., `created_date`) into standard datetime formats for time-series analysis.


* **Exploratory Analysis**:
* Identifies top-performing channels based on view counts (e.g., Cocomelon - Nursery Rhymes).
* Analyzes channel distribution by country and category.


* **Statistical Analysis**:
* Performs **ANOVA** and **Kruskal-Wallis** tests to determine if there are statistically significant differences in view counts between different channel size groups (Small, Medium, Large).



## Dependencies

To run this notebook, you will need the following Python libraries:

* `pandas`
* `numpy`
* `matplotlib`
* `seaborn`
* `scipy`

You can install the dependencies using pip:

```bash
pip install pandas numpy matplotlib seaborn scipy

```

## Dataset

The notebook expects a ZIP file named `archive (1).zip` in the working directory. This archive should contain the following CSV files:

* `youtube_channel_info_v1.csv`
* `youtube_channel_info_v2.csv`

The dataset includes attributes such as:

* **Channel Name & ID**
* **View Count & Subscriber Count**
* **Category & Country**
* **Creation Date**
* **Video Count**

## Key Results

* **Top Channels**: The analysis identifies major global channels, with "Cocomelon - Nursery Rhymes" and "SET India" being among the highest in view counts.
* **Statistical Significance**: The Kruskal-Wallis test yielded a p-value of `0.0`, indicating a statistically significant difference in view counts across different channel size groups.

## Usage

1. Place your `archive (1).zip` file in the project root directory.
2. Open the Jupyter Notebook:
```bash
jupyter notebook youtube.ipynb

```


3. Run the cells sequentially to extract data, perform cleaning, and generate analysis.
