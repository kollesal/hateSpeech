# Project work for Python Grundlagen

## Students
Melvin Kurisunkal <br />
Oliver Tanno <br />
Salome Koller <br />

## Module
**Module name:** Python <br />
**Semester:** 2023-HS <br />
**Lecturer:** Maria Pelli <br />

## Project work

### 01 Kontext

#### Hypothesis and Data Definition
**Research Question**: To what extent can machine learning models accurately classify tweets as cyberbullying or non-cyberbullying based on the content and linguistic features, and what key features contribute the most to the classification?

**H0**: The distribution of the number of unique receiveruser_ids for each senderuser_id follows a uniform or normal distribution. There is no significant difference in the frequency of senderuser_ids based on the number of unique receiveruser_ids, suggesting that the interaction patterns are evenly spread or normally distributed across the dataset.<br /><br />
**H1**: The distribution of the number of unique receiveruser_ids for each senderuser_id **does not** follow a uniform or normal distribution. There is a significant difference in the frequency of senderuser_ids based on the number of unique receiveruser_ids, suggesting that the interaction patterns are not evenly spread or distributed across the dataset.

#### Categorization of data

**by origin**
Primary Data: We don't use primary data, as we don't collect data ourselves.
Secondary Data: The "cyberbullying_tweets.csv" File is considered as Secondary data. Source: https://www.kaggle.com/datasets/andrewmvd/cyberbullying-classification/

The User dataset that is linked to the tweet has been generated by Mockaroo.

**by accessibility**
We only use open data for this project.

**by scale of measure**
The dataset contains only nominal data. There isn't a lot of variety in the dataset.
nominal: The tweets are considered as nominal.

**by structure**
unstructured: the tweets are considered as unstructured.
semi-structured: We don't use semi-structured data.
structured data: after the web scraping and data preparation the data is saved in the MySQL Table and considered as structured.

### 02 Unifying & Transformation
We have 2 Tables: The Tweets and the Users. The Join of this 2 Tables has been done in Postgres. 

The unified and transformed files are accessible in 01_Kontext/10_datasource
**Original CSV**: cyberbullying_tweets.csv
**In Prostgres transformed CSV**: interaction_with_date_and_time.csv

Also, because we only use String variables from the main tweet dataset, and a Classification Case, we don't need to unify and tranform the Dataset.

### 03 Data Cleansing
The Distribution of the Classification has been checked, as well as the search for missing values.
**Result**: The Cyberbulling Types are distributed evenly with a slight lower amount of the class "other_cyberbullying".
There are no missing values in the dataset.

### 04 Analysis & Validation
The most part of outlier detection, descriptive statistics and Verteilungen & Standardisierung has already been made in the Step EDA. <br />
The main part of this Notebook is, to validate the H0 and H1, whom are defined in 01_Kontext.

### 05 Feature Selection & Engineering
The following Feature Engineering has been made:
- Text statistics (Average lengths of strings)
- Pattern Creation (One-Hot Encoding)
- Text Lengths

### 06 EDA
The step is so late, because we only have String values in the dataset. At first, we needed to create some Int values to make a small EDA evaluation. We kept this part short, because it doesn't analyse the original dataset and is therefore not 100% accurate because it has been created through the feature engineering.
The following analysis has been made: 
- Non Graphical Univariate EDA
- Non Graphical Multivariate EDA
- Graphical Univariate EDA
- Graphical Multivariate EDA

### 07 Anwendung in Machine Learning

### 08 Anwendung von XAI – Techniken









