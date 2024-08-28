# Portfolio 1: Analysis of an E-commerce Dataset

This repository contains my solutions for the Portfolio 1 assignment for the course COMP6200 – Data Science. The assignment involves analyzing an e-commerce dataset to extract insights and perform data cleaning, descriptive statistics, visualization, and outlier detection using Jupyter Notebook.

## Contents

- `Portfolio 1_Data Cleansing.ipynb`: The Jupyter notebook containing the questions, solutions, code, and analysis for Portfolio 1.

## Assignment Details

### Analysis of an E-commerce Dataset

We have been provided with a combined e-commerce dataset. In this dataset, each user can post a rating and review for the products they purchased. Additionally, other users can evaluate the initial rating and review by expressing their trust or distrust.

### Dataset Description

The dataset includes the following fields:

- **userId:** The user's ID
- **gender:** The user's gender
- **rating:** The user's rating towards the item
- **review:** The user's review towards the item
- **item:** The item's name
- **category:** The category of the item
- **helpfulness:** The average helpfulness of this rating
- **timestamp:** The timestamp when the rating is created
- **item_id:** The item's ID
- **item_price:** The item's price
- **user_city:** The city of the user's birth

*Note:* A user may rate multiple items, and an item may receive ratings and reviews from multiple users. The "helpfulness" is an average value based on all the helpfulness values given by others.

### Tasks and Solutions

#### Q1. Remove Missing Data
**Task:** Remove records where gender, rating, or helpfulness is missing, and where the review is 'none'.

**Actions:**

- Identified and removed records with missing values in gender, rating, or helpfulness columns.
- Removed records where the review column contains 'none'.
- Displayed the DataFrame, counted the number of null values in each column, and printed the length of the data before and after removing the missing data.

#### Q2. Descriptive Statistics
**Task:** Provide data summarization with the cleaned data.

- **Q2.1:** Total number of unique users, unique reviews, unique items, and unique categories.
  - **Actions:** Used pandas functions to calculate the number of unique values in userId, review, item, and category columns.
- **Q2.2:** Descriptive statistics (total number, mean, std, min, max) regarding all rating records.
  - **Actions:** Calculated descriptive statistics for the rating column.
- **Q2.3:** Descriptive statistics (mean, std, max, min) of the number of items rated by different genders.
  - **Actions:** Grouped the data by gender and calculated the statistics for the number of items rated.
- **Q2.4:** Descriptive statistics (mean, std, max, min) of the number of ratings received by each item.
  - **Actions:** Grouped the data by item and calculated the statistics for the number of ratings received.

#### Q3. Plotting and Analysis
**Task:** Explore the correlation between gender, helpfulness, category, and ratings.

**Actions:**

- Created box plots to visualize the relationships between gender, helpfulness, category, and ratings.
- Used seaborn and matplotlib libraries for plotting.
- Analyzed the plots to identify patterns and correlations.
- Summarized observations and explanations for each plot, providing an overall summary of the data.

#### Q4. Detect and Remove Outliers
**Task:** Define and remove outliers based on specific criteria.

**Actions:**

- Removed reviews with helpfulness no more than 2.
- Identified and removed users who rated less than 7 items.
- Identified and removed items that received less than 11 ratings.
- Printed the length of the data after performing the cleaning operations.

## Repository Structure

- `README.md`: This file, providing an overview of the repository contents and assignment details.
- `Portfolio 1_Data Cleansing.ipynb`: The main assignment file containing questions, solutions, code, and analysis.

## Contact Information

For any queries or further information, please contact me at [nafialhasan@gmail.com].
