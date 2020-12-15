# AML-2020-Final-Project

## Abstract

We designed an algorithm that predicts the ability of drugs to treat neurofibromatosis-related tumors by performing natural language processing (NLP) on a corpus of journal abstracts. By aggregating real-world data from the Children’s Tumor Foundation (CTF) and Elsevier’s Scopus database, we investigated text from abstracts relevant to 87 unique combinations of drugs and oncology indications of interest. Using bag-of-words (BoW) and term frequency-inverse document frequency (TF-IDF) representations of our text data, we implemented ordinary least squares (OLS) regressions, Lasso regressions, support vector regressors (SVR), and gradient boosting regressors (GBR). We obtained promising performance in recovering the highest number of known compounds of interest from the test data using SVR or Lasso with a BoW count representation of the data.  We believe using regressions and continuous cell viability metrics to label text data is a unique formulation of the drug prediction problem.

## assets
+ **abstracts_sorted.csv:** DataFrame with the abstracts that mentioned a condition (i.e., meningioma, schwannoma, plexiform [neurofibroma]) and drug of interest
+ **data_cell_summary.csv:** DataFrame with % viability summary statistics (mean, median, min, and max) by drug by cell line
+ **data_disease_summary.csv:** DataFrame with % viability summary statistics by drug by condition
+ **moa.csv:** DataFrame for mapping drug names to mechanisms of action (from Jess White thesis)

## code
+ **White_Vishwakarma_Project_2020.ipynb:** Jupyter notebook containing all relevant code