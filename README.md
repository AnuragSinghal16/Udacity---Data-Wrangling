# WeRateDogs Twitter Data Wrangling and Analysis

## Contents
- [Project Overview](#project-overview)
- [Methodology](#methodology)
    - [1. Data Gathering](#1-data-gathering)
    - [2. Data Assessment](#2-data-assessment)
    - [3. Data Cleaning](#3-data-cleaning)
    - [4. Data Storage](#4-data-storage)
    - [5. Data Analysis & Visualization](#5-data-analysis--visualization)
- [File Structure](#file-structure)
- [How to Use](#how-to-use)
- [Acknowledgments](#acknowledgments)

## Project Overview

This project wrangles, cleans, and analyzes the [WeRateDogs](https://twitter.com/dog_rates) Twitter archive. The goal is to produce a high-quality, tidy dataset suitable for analysis, and to extract insights about dog ratings, breed predictions, and tweet engagement.

## Methodology

### 1. Data Gathering

- Downloaded the WeRateDogs Twitter archive (`twitter_archive_enhanced.csv`).
- Downloaded image prediction data (`image_predictions.tsv`).
- Queried additional tweet metadata from the Twitter API (`tweet_json.txt`).

### 2. Data Assessment

- Performed both visual and programmatic assessment.
- Identified at least 8 quality issues and 2 tidiness issues, such as missing values, incorrect data types, and the need to combine columns.

### 3. Data Cleaning

- Removed retweets and duplicates.
- Fixed data types and cleaned invalid dog names.
- Combined dog stage columns into a single column.
- Standardized breed names and filtered predictions.
- Selected relevant columns for analysis.

### 4. Data Storage

- Merged cleaned datasets into a master DataFrame.
- Saved the final dataset as `twitter_archive_master.csv`.

### 5. Data Analysis & Visualization

- Explored most common dog breeds, rating trends by dog stage, and engagement metrics.
- Created visualizations (e.g., bar charts of top breeds).
- Summarized findings in an HTML report.
