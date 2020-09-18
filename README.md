# Snapchat Political Ads
Exploring Snapchat political ads data and building a simple linear regression model to predict the number of impressions on a given ad 

## Background
Snap Inc provides data on all political and advocacy-related advertisements shown on Snapchat with the aim of increasing the level of transparency on the platform. The Snap Inc. Political and Advocacy Ads Library contains all political, issue, and advocacy ads along with relevant information on impressions, spend, and paying entities. By using the Snapchat Ads datasets from 2018 and 2019, this project addresses the vital need to understand how political organizations use social media to spread their messages to potential voters

## Project Overview
This project is split into two sections. 
#### EDA 
The first section focuses on the characteristics of advertisements that are lacking a specified end date (ads that run indefinitely) through:
* ***Cleaning and EDA***: Clean and preprocess the data along with conducting uni and bivaraite exploration of features in the data to discover associations/trends
* ***Missingness and Imputation***: Assess and handle missing values in the dataset. Perform permutation tests with *Candidate Ballot Information*, which has non-trivial missing data, to analyze the dependency of its missingness on other columns. 
* ***Hypothesis Testing***: Perform hypothesis tests to determine the characteristics of ads without a specified end date
#### Modeling
The second section is focused on developing a model to predict the number of Impressions aka the number of views through:
* ***Baseline Model***: Build a baseline linear regression model based on information we would know when an ad was launched (can't use spend or impressions as they are not determined until the ad campaign ends). 
* ***Final Model***: Engineer several features and create an sklearn ML-pipeline to search for the best model and parameters
* ***Fairness Evaluation***: Evaluate model fairness on ads with extremely low or high impressions through permutation testing
