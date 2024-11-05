# Impact of video game ratings on sales and regional sales differences

This repository contains a data analysis project exploring how product ratings affect sales and examining regional variations in sales figures. The findings aim to provide insights into the relationship between customer feedback and sales performance across different markets.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Objectives](#objectives)
- [Installation](#installation)
- [Usage](#usage)
- [Methodology](#methodology)
- [Results](#results)
- [Contributing](#Contributing)

## Overview

This project seeks to answer two main questions:
1. **How do product ratings impact sales?** Understanding this relationship can reveal the extent to which customer feedback influences buying behavior.
2. **Are there notable differences in sales across regions?** This can uncover regional trends and help tailor sales strategies to each market.

The repository includes the notebook and resources to replicate the analysis, visualizations, and findings.

## Dataset

### Video Game Sales Data
The file at [this link](https://g-schmit.github.io/data/vg_sales.csv) contains data on video game sales. It was obtained from [Kaggle](https://www.kaggle.com/datasets/gregorut/videogamesales) and includes the following information:

| Column Name   | Description                                    |
|---------------|------------------------------------------------|
| **Rank**      | The rank of the game in sales                  |
| **Name**      | The name of the game                           |
| **Platform**  | Platform on which the game was released (PC, PS4, etc.) |
| **Year**      | Year of release                                |
| **Genre**     | Genre of the game                              |
| **Publisher** | Publisher of the game                          |
| **NA_Sales**  | Sales in North America (in millions)           |
| **EU_Sales**  | Sales in Europe (in millions)                  |
| **JP_Sales**  | Sales in Japan (in millions)                   |
| **Other_Sales** | Sales in the rest of the world (in millions) |
| **Global_Sales** | Total global sales                          |

### MetaCritic Scores Data
Another file is available at [this link](https://g-schmit.github.io/data/all_meta_games.csv). In this file, we can find the MetaCritic scores of games published from 1995 to 2021. This file can help determine links between sales and game scores. It contains the following information:

| Column Name   | Description                                    |
|---------------|------------------------------------------------|
| **name**      | The name of the game                           |
| **platform**  | Platform on which the game was released        |
| **release_date** | Release date                                |
| **summary**   | Summary of the game                            |
| **meta_score** | Score given by MetaCritic                     |
| **user_review** | Score given by users                         |

## Objectives

The objective here is to analyze these data together in order to :

1. **Impact of Ratings on Sales**
   - Explain if the ratings of games (MetaCritic and user reviews) have an impact on global and regional game sales.

2. **Differences in Sales by Region**
   - Explain the differences in sales by region (North America, Europe, Japan, and the rest of the world).

We will also look for other external data sets in order to rich our existing data to have better results, and in order to apply supplimentary tests.

## Installation

To use this repository locally, clone the repo and install the dependencies.

```bash
git clone https://github.com/your-username/Impact-of-Ratings-on-Sales.git
cd Impact-of-Ratings-on-Sales
```

## Usage

1. Open the Jupyter Notebook:
```bash
jupyter notebook Games_rates_on_sales_SALEEM.ipynb
```
2. Run each cell in sequence to follow the data loading, cleaning, analysis, and visualization steps.

## Methodology

This analysis follows a structured approach:

1. **Data Loading**: Import the video game sales and MetaCritic scores datasets into the notebook.
2. **Exploration & Cleaning**: Conduct exploratory data analysis (EDA) and handle any missing values or inconsistencies to ensure data quality.
3. **Unification & Merging**: Merge the sales and ratings datasets to create a unified dataset for analysis.
4. **External Data Integration**: Integrate additional relevant data to enrich the dataset.
5. **Data Preparation**: Prepare the data by creating new features, encoding variables, and setting up for statistical analysis.
6. **Analysis**: Perform statistical and graphical analyses to investigate:
   - The correlation between ratings and sales.
   - Differences in sales by region.

## Results

### Impact of Ratings on Sales

- **Correlation Between Ratings and Global Sales**: The analysis found statistically significant correlations between ratings and global sales (p-values < 0.05). This suggests a moderate relationship, where higher ratings are associated with increased global sales.
- **Observations from Plots**: Visualizations indicate that as user and MetaCritic reviews increase, there is a corresponding rise in global sales, implying that positive feedback may contribute to higher sales figures.

### Regional Sales Differences

- **Regional Preferences**: Different regions exhibit distinct preferences for games and platforms. In Japan, Nintendo and PlayStation dominate, while in North America and Europe, a variety of platforms, including Xbox, show strong sales.
- **Peak Sales Period**: The period from 2005 to 2010 marked a peak for global game sales, largely due to the release of popular consoles and major game titles that resonated across various markets.

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch.
3. Make changes and submit a pull request.

