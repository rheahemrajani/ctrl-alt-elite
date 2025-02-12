# Sentiment Trends in U.S. Airline Twitter Data

## Contents of the Repository
This repository contains all files and documentation related to Sentiment Trends in US Airline Twitter Data. Below is a breakdown of its contents:

- `SCRIPTS/` - Contains all code/scripts used for data processing, analysis, or model execution.
- `DATA/` - Includes raw and processed data files used in the project.
- `OUTPUT/` - Stores all results generated from running the scripts.
- `README.md` - This file, providing an overview of the project.
- `LICENSE.md` - The license file (MIT by default).

## Software and Platform
To run this project, you will need the following software and dependencies:

- **Programming Language:** Python 3.x
- **Packages Required:**
  - [`pandas`](https://pandas.pydata.org/) - For data manipulation and analysis
  - [`VADER (nltk.sentiment)`](https://github.com/cjhutto/vaderSentiment) - For sentiment analysis
- **Platform:** Tested on macOS

To install the necessary dependencies, run:

```bash
pip install pandas vaderSentiment

## Project Folder Structure
project-folder/
│-- SCRIPTS/          # Source code and scripts
│-- DATA/             # Raw and processed data files
│-- OUTPUT/           # Generated results
│-- README.md         # Project overview
│-- LICENSE.md        # MIT license information

## Reproducing the Results
To reproduce the results of this project, follow these steps:

### 1. Clone the Repository
First, download the repository to your local machine:
```bash
git clone https://github.com/rheahemrajani/ctrl-alt-elite.git
cd ctrl-alt-elite
### 2. Install Dependencies
pip install pandas vaderSentiment scikit-learn
### 3. Download and Prepare Data
The dataset, Tweets.csv, was originally obtained from Kaggle and is included in the DATA/ folder of this repository.
The cleaned dataset Clean_Tweets.csv will be saved in the DATA/ folder.
### 4. Perform Sentiment Analysis (VADER)
Run the sentiment analysis script:
python SCRIPTS/vader_analysis.py
This script:
Applies VADER sentiment analysis to the cleaned tweets.
Extracts and compares the VADER scores to the original sentiment scores in the dataset.
Focuses on tweets with negative sentiment values.
### 5. Perform TF-IDF Analysis
To analyze word frequency, run:
python SCRIPTS/tfidf_analysis.py
This script:
Uses TF-IDF (Term Frequency-Inverse Document Frequency) to identify the most common words in the dataset.
Helps determine which words contribute most to negative sentiment scores.
### 6. Run Linear Regression Analysis
To examine the correlation between frequent words and sentiment scores:
python SCRIPTS/linear_regression.py
This script:
Uses TF-IDF results to identify the most common words.
Performs a linear regression to check if frequently occurring words correlate with higher negative sentiment scores.
### 7. View Results
The results, including sentiment analysis outputs and regression results, will be stored in the OUTPUT/ folder.
Key figures, CSVs, and analysis summaries can be found there for further exploration.

