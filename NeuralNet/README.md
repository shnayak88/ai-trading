# Analyzing Stock Sentiment from Twits
Build a deep learning model to classify the sentiment of messages from StockTwits, a social network for investors and traders. The model will be able to predict if any particular message is positive or negative. From this, it'll be able to generate a signal of the public sentiment for various ticker symbols.

Instructions:
1) Import twits and split the message into message body and sentiment 
2) Pre-process the data: use regex to remove specific words or phrases
3) Bag of Words: Create a vocabulary and count up how often each word appears in our entire corpus
4) Remove some of the most common words such as 'the', 'and', 'it. Remove really rare words as well 
5) Now we have our vocabulary which means we can transform our tokens into ids, which are then passed to our network. 
   Here is a nice diagram showing the network we'd like to build:
    # Embed -> RNN -> Dense -> Softmax
6) Run the model on train and test data 
