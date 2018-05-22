# Sentiment-Analysis

Predict the sentiment of tweets

Problem statement: 
To determine the sentiment of a given tweet. To classify whether a given tweet is expressing the positive or negative view about the topic .
INPUT : Tweets from twitter
OUTPUT: Positive or Negative Label to the tweet 

Motivation: To get the opinion of peoples on any topic, product, issue etc. Any organisation would want to know how people are reacting to its product or services Based on a sample of tweets. 

Labels: 
Generally a binary opposition in opinion is assumed.
For/Against, Like/Dislike, Good/Bad, Positive/Negative.
So we have Two Labels of Sentiments Positive and Negative.

Methodology/Algorithm:     
1. Pre-process tweet into tokens.
2. Remove hash tag, hyperlinks, stopwords using NLP.
3. Used word2vec neural network model to convert every token into vector 
4. Multiplying every word with its tf-idf score and taking average over the sum of all tokens(words) in specific tweet to make     sent2vec (vectors for sentence).
5. Training on sequential deep neural network (using Keras).
6. Collecting new tweets from Twitter to predict sentiment. 
7. Displaying the tweets with Positive and Negative sentiment and Accuracy of model.  

result:
output the tweets with positive and negative labels.

Conclusion: 
1. Dataset must be larger for trainnig.
2. It performs fairly well within same dataset.
3. Though it performs very well within the same dataset it doesn’t perform very well with new random tweets.
4. Deep Neural Network perform better than other machine learning models like Naive Bayes. 

Dataset:
1. Dataset 1 from stanford contains 1.6 million tweets with sentiment derived by emoticon. 
2. Dataset 2 from Sanders Analysis contains 1.57 million tweets with hand-classified sentiments. 

Reference:
Research papers:
1) A survey of sentiment analysis techniques  https://ieeexplore.ieee.org/document/8058315/ 
2) A Comparison between Preprocessing Techniques for Sentiment Analysis in Twitter  ​https://ceur-ws.org/Vol-1748/paper-06.pdf

Articles:
1) https://www.youtube.com/watch?v=si8zZHkufRY&t=501s
2) https://blog.griddynamics.com/creating-training-and-test-data-sets-and-preparing-the-data-for-twitter-stream-sentiment-analysis-of-social-movie-reviews/
3) http://www.awesomestats.in/python-sentiment-tweets/
3 )http://cv-tricks.com/tensorflow-tutorial/save-restore-tensorflow-models-quick-complete-tutorial/4) https://www.kaggle.com/c/word2vec-nlp-tutorial#part-1-for-beginners-bag-of-words

