Movie_Rating_Prediction
=======================
Movie ratings are predicted from the recent twitter feed. A Linear SVC model is trained using the training dataset from the Stanford AI lab’s “Large Movie Review Dataset”. This model is used for sentiment analysis of each tweet thereby classifying it as positive or negative and accordingly a rating is assigned for the tweet.

Simulation
=======================

###Packages Required
1) [scikit-learn](http://scikit-learn.org/stable/) 

The train_classier.ipynb trains a Linear SVC classifier using a Count Vectorizer for feature extraction. The vectorizer and the classifier are saved using pickle in order to be used for the twitter data.

The movie_rating.ipynb gets the tweets for the movie and finds sentiment using the trained classier and then converts that sentiment to a rating value. It also gives the IMDB rating of that movie.

