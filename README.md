# Differentiating between Physics and Astronomy

## A lot of times Physics and Astronomy can seem very similar but can a NLP model distinguish between two?

## Solution: 
- Data: PushShift's API was used to get data from reddit posts
- Data cleaning: Some posts didn't have the body of the text, or it was deleted or removed. These were filtered out and substituted by an empty string
- Data preprocessing: The final variable, the title and the body strings together, were then tokenized and lemmatized to bring them to their base
- Model 1: Countvectorizer and Multinomial Naivë Bayes. The model performed well with the accuracy scores: 0.89 for training and 0.87 for testing.
- Model 2: TF-IDF and Multinomial Naivë Bayes. The model performed well with the accuract scores: 0.89 for training and 0.875 for testing.
- Model 3: Countvectorizer and Random Forest. The model was severly overfit with the scores: 0.97 for training and 0.86 for testing.
