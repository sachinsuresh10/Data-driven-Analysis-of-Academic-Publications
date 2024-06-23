# Data-driven-Analysis-of-Academic-Publications

## Overview

This project involves analyzing a dataset containing abstracts from 4385 research papers published between 2000 and 2022 by three major journals: 
- [Journal of the Operational Research Society](https://www.tandfonline.com/journals/tjor20)
- [Health Systems](https://www.tandfonline.com/journals/thss20)
- [Journal of Simulation](https://www.tandfonline.com/journals/tjsm20)

The dataset includes details such as the paper's title, journal name, year of publication, number of pages, list of authors, number of views, number of citations, altmetric score, and the abstract.

## Highlights

This study explores the dataset to identify interesting patterns and draw general conclusions. The analysis involves:
- Bag of Words and TF-IDF for identifying popular words.
- Topic Modelling using LDA to uncover hidden topics.
- Regression Analysis to predict citation counts.
- Classification to predict journal categories.
- Association Rule Mining to find word associations.
- Clustering to identify similar abstracts.
- Dimensionality Reduction using PCA to visualize clusters.

## INDEX

1. Introduction
    - Dataset Overview
    - Objectives of Analysis
2. Data Pre-Processing
    - Loading and Cleaning
    - Text Data Transformation
    - Document-Term Matrix (DTM) Creation
    - TF-IDF Transformation
3. Exploratory Data Analysis (EDA)
    - Visualizations Overview
    - Word Cloud
    - Yearly Trends
    - Top Terms Visualization
4. Topic Modelling (LDA)
    - Model Description
    - Optimal Topic Number Search
    - Visualization of Topics
5. Regression Analysis
    - Multiple Regression Model
    - Key Predictors and Coefficients
6. Classification Analysis
    - Model Overview
    - Accuracy Evaluation
7. Association Rule Mining
    - Binary Matrix Transformation
    - Apriori Algorithm Application
8. Clustering Analysis
    - Cluster Identification Method
9. Dimensionality Reduction (PCA)
    - PCA Overview
10. Conclusion

## 1. Introduction

This analysis examines a dataset of 4385 research papers from three major journals published between 2000 and 2022. The objective is to explore the abstracts and associated details to uncover trends, significant topics, and factors influencing attention and impact.

## 2. Data Pre-Processing

The dataset was preprocessed to ensure cleanliness and readiness for analysis:
1. **Loading and Cleaning**: Loaded the dataset and removed rows with missing values using `na.omit()`.
2. **Text Data Transformation**: Created a corpus, converted text to lowercase, removed punctuation, numbers, and common stop words, and stripped unnecessary whitespaces.
3. **Document-Term Matrix (DTM) Creation**: Structured the abstracts into a DTM to capture term frequencies.
4. **TF-IDF Transformation**: Applied TF-IDF to highlight important terms within the corpus.

## 3. Exploratory Data Analysis (EDA)

We conducted a thorough examination and visualization of the dataset:
1. **Word Cloud**: Visual representation of popular words in the abstracts.
2. **Yearly Trends**: Plots illustrating the variation of views and citations across different years.
3. **Top Terms Visualization**: Plots comparing Term Frequency (TF) and TF-IDF.

## 4. Topic Modelling (LDA)

Using Latent Dirichlet Allocation (LDA), we uncovered hidden topics within the abstracts:
1. **Model Description**: Statistical model to uncover hidden topics.
2. **Optimal Topic Number Search**: Determined using metrics like CaoJuan2009 and Deveaud2014.
3. **Visualization of Topics**: Showcased the distribution of topics over time and across journals.

## 5. Regression Analysis

A multiple regression model was built to predict the number of citations a new abstract might receive, considering predictors like views and altmetric scores.

## 6. Classification Analysis

Developed a model to predict the journal category of a paper based on its features, and evaluated the model's accuracy.

## 7. Association Rule Mining

Converted the abstracts into a binary matrix and applied the Apriori algorithm to identify meaningful word associations, using a support threshold of 0.1 and a confidence threshold of 0.8.

## 8. Clustering Analysis

Applied clustering methods to group similar abstracts and identified top words in each cluster based on TF-IDF scores.

## 9. Dimensionality Reduction (PCA)

Applied PCA to reduce dimensionality and visualized the data clusters in a 2D space.

## 10. Conclusion

Key findings from the analysis:
1. **Bag of Words and TF-IDF**: Identified popular words and their significance across different years and journals.
2. **Topic Modelling (LDA)**: Uncovered hidden topics and their evolution over time.
3. **Regression**: Predicted citation counts and identified influencing factors.
4. **Classification and Association**: Predicted journal categories and explored word associations.
5. **Clustering**: Identified distinct clusters and their characteristics.
6. **PCA**: Visualized data clusters to understand abstract patterns and relationships.

The analysis provides a comprehensive understanding of the dataset's content, impact, and categorization, offering practical implications for researchers, journals, and academic decision-makers.

## How to Run

1. **Data Download**:
    - Download the dataset from Blackboard.

2. **Pre-processing and Analysis**:
    - Use the provided R and Python scripts for data cleaning, imputation, visualization, regression, classification, clustering, and PCA.

## Dependencies

- R
- Python
- Pandas
- Scikit-learn
- XGBoost
- Matplotlib
- Seaborn

