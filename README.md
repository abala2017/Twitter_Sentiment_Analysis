# Twitter_Sentiment_Analysis
 In this project I tried to get the sentiment from Twitter Tweets. The dataset I used came from a Kaggle dataset (https://www.kaggle.com/kazanova/sentiment140). The dataset was labelled with with either 0 = negative sentiment, 2 = neutral sentiment, or 3 = postive sentiment. Before putting it into a model, I had to preprocess the tweets, which involved things such as finding a way to replace the emojis, getting rid of some of the extrenuous punctuation, and etc. To interpret the tweets, I could have done a one-hot vector, but that would be very computationally expensive. Instead I opted for using GloVe Vectors to represent each word. I used the pre-trained vectors from Stanford's Twitter vocabulary (https://nlp.stanford.edu/projects/glove/). In which they have a vocabulary of around 1.2 million words. In order to predict which sentiment a tweet had I used a Recurrent Neural Network with LTSM cells. Using this RNN we get an accuracy of 83% on training and 82% on testing. There are still some potential areas I could work on to increase accuracy which I will come back to work on at a later time.
