# Duolingo App Reviews Sentiment Analysis Project

## Table of Contents

- [Introduction](#introduction)
- [Project Overview](#project-overview)
- [Skills and Tools](#skills-and-tools)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Data Collection](#data-collection)
- [Data Preprocessing](#data-preprocessing)
- [Sentiment Analysis](#sentiment-analysis)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Results](#results)
- [Conclusion](#conclusion)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This repository contains the code and resources for a sentiment analysis project conducted on user reviews of the Duolingo language learning app. The project involves scraping user reviews from the Google Play Store, performing sentiment analysis using the VADER lexicon, and conducting exploratory data analysis to gain insights into user sentiments and trends.

## Project Overview

The main goals of this project are as follows:

1. Collect a substantial number of user reviews for the Duolingo app from the Google Play Store using the 'google_play_scraper' API.
2. Preprocess the collected reviews by converting them to lowercase, removing special characters, and preparing them for sentiment analysis.
3. Perform sentiment analysis on the reviews using the VADER lexicon from the NLTK library to classify them as positive, negative, or neutral.
4. Conduct exploratory data analysis to analyze review lengths, sentiment strength distributions, and common words in each sentiment group.

## Skills and Tools

- Python
- Data scraping using 'google_play_scraper'
- Data preprocessing
- Sentiment analysis with NLTK's VADER lexicon
- Exploratory data analysis
- Data visualization using libraries like Matplotlib and Seaborn

## Data Collection

The 'google_play_scraper' API is used to scrape user reviews for the Duolingo app from the Google Play Store. Multiple batches are collected using loops to gather thousands of reviews. The collected data is stored in a pandas DataFrame.

## Data Preprocessing

Reviews are preprocessed to convert them to lowercase, remove special characters, and prepare them for sentiment analysis. A feature preprocessing pipeline is used to streamline this process.

## Sentiment Analysis

Sentiment analysis is performed using the VADER lexicon from NLTK. The SentimentIntensityAnalyzer class is employed to classify reviews as positive, negative, or neutral.

## Exploratory Data Analysis (EDA)

EDA is conducted to explore various aspects of the data. Review lengths are analyzed and visualized by sentiment group. Sentiment strength distributions are visualized, and common words for each sentiment group are identified.

## Results

The results of the sentiment analysis and exploratory data analysis are as follows.
1. Negative reviews seem to be longer in length while neutral reviews (usually containing irrelevant or absurd remardks) are rather short
2. Positive reviews tend to be 'stronger' positively than negative reviews are negatively
3. Negative reviews seem to contain more grammatical errors
4. Negative reviews can also be seen as non-serious humor in some cases, with many references comically to the Duolingo Owl

Thr grouped sentiment reviews could be further explored for specific feature insights and consumer pain points. 

## Conclusion

This project showcases the process of collecting, preprocessing, and analyzing user reviews from the Duolingo app. The sentiment analysis and exploratory data analysis provide valuable insights into user sentiments and can guide app improvements and user engagement strategies.
