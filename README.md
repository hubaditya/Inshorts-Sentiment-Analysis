# Inshorts-Sentiment-Analysis
 A sentiment analysis using Affin and TextBlob lexicon on feeds scraped from a news website through Beautiful Soup analysing constituency parsing, POS tagging and Named Entity recognition
 
 ### Motivation
 Often news when grouped together can tell how the current scenario is unfolding in the world. Which industry is feeling the heat, which industry is flourishing or getting in general the sentiment of the public can be used in further analyses by the businesses relevant in those industry and identify scope of improvements.<br>
 This project aims to fetch the sentiments of the news currently trending in different industries from [inshorts](https://www.inshorts.com/)
 
 ### Problem Statement
 Develop a sentiment analysis on sports, technology and overall industry
 
 ### Dataset
 The data was scraped from the inshorts website using Beautiful Soup across three categories - sports, technology and world
 
| Column            | Description         | Data Type |
|:---               |:---                 |:----------|
| news_headline     | news heading        | String   |
| news_article      | news description    | String   |
| news_category     | industry            | String   | 

### Technical Details

#### Libraries
* pandas & numpy - for data wrangling and mathematical operations
* matplotlib and seaborn - for rich data visualization
* requests and bs4 - for scraping data
* re and unicode - for data cleaning
* nltk and spacy - for data cleaning, tokenization and analysing constituency parsing, POS tagging and Named Entity recognition
* afinn and textblob - for calculating sentiment analysis

#### Feature Engineering
* stripped HTML tags
* expanded contractions using a custom built mapping
* removed accented characters to ASCII values
* text lemmatization for capturing fundamental context
* removed noise from the corpus like special characters, stopwords and numeric characters

#### Data Exploration
* parts of speech tagging
* chunking the text corpus for further identification
* created a dependency parsing to explore relation between words of a sentence
* Named Entity Recognition for visualizing the entities in the corpus

### Modeling
Using Afinn and TextBlob algorithms for get polarized scores of news

### Result
Sports industry had more positive news which could be related to India's current top performance in sports, tech industry was neutral with some positive and some negative news. The wordly news was most negative owing to the coronavirus.
![sentiment-category](https://github.com/hubaditya/Inshorts-Sentiment-Analysis/blob/main/news%20sentiment%20category.png)
![sentiment](https://github.com/hubaditya/Inshorts-Sentiment-Analysis/blob/main/news%20sentiment.png)


