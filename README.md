# dataSciProj
SC1015 mini project
This project aims to predict the direction of stock market movement based on the top 25 news headlines daily. 

The stock market is represented by the daily closing price of the Dow Jones Industrial Average (DJIA), one of the main indicators of the US economy.  The stock movement is denoted by 1, having increased or remained the same, where as 0 as having decreased from the previous day.

1. Cleaning
We cleaned our data by removing punctuations, converting all texts into lower case and removing special characters. We also used some advanced natural language processing tools to simplify and standardize text, to help the program understand and process language more effectively. These include tokenisation, which breaks down text into simpler form, and removing numbers and stop words which are filler words. Lastly, we combined the headlines for each day into one column for easier analysis later on.

Then, we got the sentiment score of each date's headlines. This is important in finding a correlation between the news headlines and stock market movement.

From the data, we also implemented our own statistics such as 7-day average, 30-day average, daily price returns (daily profit or loss) and 30-day volatility. 

2. Exploratory data analysis
We utilised various Exploratory Data Analysis Techniques

3. Machine Learning
We used multiple machine learning models to predict the stock market. Firstly, we attempted predicting the stock market using our sentiment_score values derived from DataCleaning.ipynb. We used a simple model to predict this, as well as a decision classification tree. This showed little promise in prediting stock prices.

Going forward, we decided to use TF-IDF (Term Frequency-Induced Document Frequency) as a measure to evaluate the words in the document. Firstly, we used TF-IDF with n-grams (n words per sequence) in a Logistic Regression model. Then, we also tried using Random Forest and Gradient Boosting to predict the stock market movement.

The results show that the stock market is influenced by numerous factors, such as politics and policies, global events, investor psychology, market speculation, etc. This highlights the complexity of financial markets. While the project did not yield the desired predictive success, it provided valuable insights into the interplay between news sentiment and market behavior, paving the way for further research using more diverse data sources and advanced modeling techniques. Furthermore, we were able to learn and explore the growing field of Natural Language Processing.
