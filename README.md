Movie_Rating_Prediction
=======================
Movie ratings are predicted from the recent twitter feed. A Linear SVC model is trained using the training dataset from the Stanford AI lab’s “Large Movie Review Dataset”. This model is used for sentiment analysis of each tweet thereby classifying it as positive or negative and accordingly a rating is assigned for the tweet.

Packages Required
=======================
1) [Scikit-Learn](http://scikit-learn.org/stable/) 

2) [NLTK](http://www.nltk.org/)

3) [Enchant](https://pythonhosted.org/pyenchant/tutorial.html)

4) [Twitter](https://pypi.python.org/pypi/twitter)

5) [IMDB](http://imdbpy.sourceforge.net/)

Simulation
=======================
The datasets can be obtained from [here](http://ai.stanford.edu/~amaas/data/sentiment/)

The train_classier.ipynb trains a Linear SVC classifier using a Count Vectorizer for feature extraction. The vectorizer and the classifier are saved using pickle in order to be used for the twitter data.

The replacers.py helps in pre-processing of text for term expansion, repeated character removal and spell checker.

The movie_rating.ipynb gets the tweets for the movie and finds sentiment using the trained classier and then converts that sentiment to a rating value. It also gives the IMDB rating of that movie.

