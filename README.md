
# Stock price movement prediction from news headlines - NLP

Use natural-language processing (NLP) to predict stock price movement based on News headlines.


## Aim

This project aims to use natural language processing (NLP) and sentiment analysis to predict the direction of a company's stock price based on news headlines. We will be analyzing various types of news articles to determine the sentiment of the headlines and use this information to predict whether the stock price is likely to increase or decrease.


## Dataset used

- The Dataset in consideration is a combination of the world news and stock price shift available on Kaggle.
- There are 25 columns of top news headlines for each day in the data frame.
- Data ranges from 2008 to 2016 and the data from 2000 to 2008 scrapped from yahoo finance.
- Labels are based on the Dow Jones Average stock index.
    - class1 -- The stock price increased.
    - class0 -- The stock price decreased.
## Requirement

- Python 3.9
- numpy

## Methodology

-This project involves three steps for predicting stock price movement from news headlines: data preprocessing, model training, and prediction and analysis.

 1. Data Preprocessing: In this step, we will clean and prepare the news headlines data for modeling.


2. Train Model: Next, we will use the preprocessed data to train a predictive model.

3. Prediction and Analysis: Finally, we will use the trained model to make predictions on unseen data and analyze the results.
#### Data Preprocessing

- Handling the null values
- seperating train test data. Here train data is taken from year 2000 to 2015 and the test data is taken from year 2014 to 2016.
- Removing special characters, converting all letters to lower case and concatinating 25 columns containing text into single list called headlines.
- Converting text to token using CountVectoriser.
#### Creating and Training Model

In this project, we will be using the Random Forest Classifier to train our model. We will set the hyperparameters n_estimators to 200 and criterion to 'entropy' for the classifier.
#### Prediction and Analysis

After training the model, we used it to generate predictions. The model achieved an accuracy score of 85% on the training data.
