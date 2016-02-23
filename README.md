# yelp-data-challenge

This repository demonstrates how to build a predictive model using Yelp review data. The main result is a multinomial Naive Bayes model that predicts the star rating of a Yelp review using only its text content. We utilize NLP techniques including bag of words representation, stemming, and count vectorization to preprocess the data. A class imbalance problem is overcome through the use of a a custom up-sampling and cross validation routine to determine the optimal over sampling rate. The analysis is contain in ipython notebooks.

### Using the code

There are 2 main scripts:
  1.  *preprocessing.ipynb* contains the code to clean the text data and get it ready for modeling. We remove stop words, puncuation and other non-important parts of the text. We also transform the data into its bag of words representation using the sklearn count vectorizer. 
  2.  *model_selection.ipynb* contains the code to build the multinomial naive bayes classification model and a custum over sampling routine that includes a method for cross validation and finding an optimal over sampling rate. There is also some exploration of word clustering techniques. 
