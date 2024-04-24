# Data Science Project
SC1015 mini project

# Introduction
This project aims to predict the direction of stock market movement based on the top 25 news headlines daily. 

The stock market is represented by the daily closing price of the Dow Jones Industrial Average (DJIA), one of the main indicators of the US economy.  The stock movement is denoted by 1, having increased or remained the same, where as 0 as having decreased from the previous day.

# 1. Cleaning
We cleaned our data by removing punctuations, converting all texts into lower case and removing special characters. We also used some advanced natural language processing tools to simplify and standardize text, to help the program understand and process language more effectively. These include tokenisation, which breaks down text into simpler form, and removing numbers and stop words which are filler words. Lastly, we combined the headlines for each day into one column for easier analysis later on.

Then, we got the sentiment score of each date's headlines. This is important in finding a correlation between the news headlines and stock market movement.

From the data, we also implemented our own statistics such as 7-day average, 30-day average, daily price returns (daily profit or loss) and 30-day volatility. 

# 2. Exploratory data analysis
We utilised various Exploratory Data Analysis Techniques such as box plot and scatter plot as taught in the course. We also learnt an interesting data visualisation tool: Word Cloud

## a. Boxplot:
We visualised the distribution of sentiment scores, revealing that the majority of the data falls within a narrow range of 0.0 to 0.7, with an even tighter concentration between -0.15 and 0.2. Despite sentiment scores theoretically ranging from -1 to 1, this limited variability suggests a challenge in discerning extreme sentiments from the data. To normalize the data for further analysis, outliers were removed.

## b. Scatter Plot:
Another EDA technique involved plotting sentiment scores against the average stock prices over both 7 and 30 days. Surprisingly, the correlation between sentiment and stock prices was found to be minimal, with a correlation coefficient of -0.06. This lack of correlation was consistent regardless of whether analysing shorter-term (7-day) or longer-term (30-day) stock movements.

## c. Word Cloud:
To gain insights into the textual content of headlines and its potential impact on sentiment, we employed word cloud visualisation. This method provides a visual representation of word frequency and importance within the headlines. Words appearing more frequently are depicted with larger sizes, offering a glimpse into the prevailing themes and sentiments conveyed in the headlines.

These EDA techniques collectively aimed to uncover patterns and relationships within the data, facilitating a deeper understanding of the dynamics between news sentiment and stock market movements.

# 3. Machine Learning
We used multiple machine learning models to predict the stock market. Firstly, we attempted predicting the stock market using word frequency, with our baseline model.
we also our sentiment_score values derived from DataCleaning.ipynb. We used a decision classification tree. This showed little promise in prediting stock prices.

Going forward, we decided to use TF-IDF (Term Frequency-Induced Document Frequency) as a measure to evaluate the words in the document. Firstly, we used TF-IDF with n-grams (n words per sequence) in a Logistic Regression model. Then, we also tried using Random Forest and Gradient Boosting to predict the stock market movement.

The results show that the stock market is influenced by numerous factors, such as politics and policies, global events, investor psychology, market speculation, etc. This highlights the complexity of financial markets. While the project did not yield the desired predictive success, it provided valuable insights into the interplay between news sentiment and market behavior, paving the way for further research using more diverse data sources and advanced modeling techniques. Furthermore, we were able to learn and explore the growing field of Natural Language Processing.

# References

https://www.kaggle.com/datasets/aaron7sun/stocknews

# Contributions
Work divided equally among See Tow, Jordan and Ren Kai
@Paxton2001
@jordi2987
@kohrenkai
