# HuobiSentimentAnalysis
## Sentiment Analysis of a Telegram Channel focused on Cryptocurrencies with PySpark
In the current study, the Telegram channel “Huobi English” is analyzed using PySpark. Huobi Global, the company behind this channel, is a cryptocurrency exchange company with headquarters in Seychelles. The channel is focused on discussing the latest trends in the cryptocurrency market, as well as serving as a platform for Huobi users to communicate with the company. The company has set up a Telegram bot to regularly announce channel rules and convenient trends, as well as a series of channel administrators who can respond to user’s questions and complaints. The channel is completely open to any Telegram user that has the channel’s address.

In order to analyze this channel, a dataset containing all of the channel’s posts during a specific time interval has been used. This dataset has been extracted via the Telegram API and the Telethon Python Module by a Kaggle User, and has been made available in the attached post (https://www.kaggle.com/aagghh/crypto-telegram-groups?select=group_messages_huobi.json). In the post, the corresponding datasets of other four Telegram channels of a similar nature are also presented. However, due to its adequate size, only the dataset corresponding to “Huobi English” was selected.

Given this dataset, the task of this study is to extract valuable data from the channel’s posts, in particular regarding the daily and weekly distribution of channel activity, the number of times each one of the most popular cryptocurrencies is mentioned, and the evolution of channel sentiment with time. As a reference, the market prices of each of the analyzed currencies are taken into account. All of these insights are to be obtained while leveraging the power of PySpark, with particular focus in the API’s SQL functions, and Spark NLP.

As a result, the current study sets out to answer the following questions based on the presented dataset:
* What fields of the dataset are relevant to the current study? What is the number of missing and null values in each of them?
* What are the days of the week and the hours of the day with greatest channel participation?
* What are the most mentioned cryptocurrencies? What is the evolution of these mentions over time?
* Is the evolution of channel mentions of a crytpocurrency with time related to the evolution of its price?
* What is the evolution of the channel’s sentiment with time? Does this evolution hold any relationship with relevant cryptocurrency prices?
* Can channel sentiment be obtained with Spark NLP's pretrained models?
* Can one predict the evolution of relevant cryptocurrency prices based on the sentence and word embeddings of each post? Is this done better with a NN via PyTorch or with Spark NLP's ClassifierDL?
