# Sentiment Trends in U.S. Airline Twitter Data

## Contents of the Repository
This repository contains all files and documentation related to Sentiment Trends in US Airline Twitter Data. Below is a breakdown of its contents:

- `SCRIPTS/` - Contains all Jupyter notebooks (.ipynb) used for data processing, analysis, or model execution.
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
  - matplotlib – For visualizations and plotting.
  - seaborn – For enhanced statistical visualizations.
  - vaderSentiment – For sentiment analysis using VADER.
  - sklearn (scikit-learn) – For TF-IDF analysis and regression modeling.
  - wordcloud – For generating word clouds.
  - statsmodels – For LOWESS regression and statistical analysis.
  - numpy – For numerical computations.
    
- **Platform:** Tested on macOS

To install the necessary dependencies, run:

```bash
pip install pandas vaderSentiment
pip install pandas
pip install matplotlib
pip install seaborn
pip install vaderSentiment
pip install scikit-learn
pip install wordcloud
pip install statsmodels
pip install numpy

## Project Folder Structure
project-folder/
│-- SCRIPTS/          # Jupyter notebooks for analysis
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
pip install pandas vaderSentiment scikit-learn matplotlib seaborn wordcloud statsmodels numpy
### 3. Download and Prepare Data
The dataset, Tweets.csv, was originally obtained from Kaggle and is included in the DATA/ folder of this repository.
The cleaned dataset Clean_Tweets.csv will be saved in the DATA/ folder.
### 4. Open the Jupyter Notebooks
4.1 Data Cleaning and Preprocessing
Notebook: datacleaning.ipynb
- Loads Tweets.csv from the DATA/ folder.
- Cleans and preprocesses text data.
- Saves the processed dataset (Clean_Tweets.csv) in the DATA/ folder.
4.2 Perform Sentiment Analysis (VADER)
Notebook: sentimentanalysis.ipynb
- Applies VADER sentiment analysis to the cleaned tweets.
- Extracts and compares the VADER scores to the original sentiment scores in the dataset.
- Focuses on tweets with negative sentiment values.
4.3 Perform TF-IDF Analysis
Notebook: tfidfanalysis.ipynb
- Uses TF-IDF (Term Frequency-Inverse Document Frequency) to identify the most common words in the dataset.
- Helps determine which words contribute most to negative sentiment scores.
4.4 Further Analysis and Visualizations
Notebook: furtheranalysis_visualizations.ipynb
- Generates additional visualizations, including bar charts, word clouds, and regression plots.
- Explores trends in sentiment scores across airlines.
### 5. View Results
The results, including sentiment analysis outputs and regression results, will be stored in the OUTPUT/ folder.
Key figures, CSVs, and analysis summaries can be found there for further exploration.

