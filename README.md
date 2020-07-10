# 🎭Truth Teller

**Adopted from a Kaggle Competition**

## Problem statement

Twitter as a source for timely news also presentes the challenges of what a tweet means - be it actual fact versus metaphor. As the platform has been crucial in [detecting earthquakes in real time](https://www3.nd.edu/~dwang5/courses/spring15/papers/media-sensing/twitter-earthquake.pdf), it is also the case that some tweets don't mean what they say. For instance, [this tweet](https://twitter.com/AnyOtherAnnaK/status/629195955506708480) "uses the word 'ABLAZE' but means it metaphorically" (1).

In order for machines to be able to automatically detect tweets that are relevant each tweet has to be classified as either describing a real disaster not, denoted as **1** and **0** respectively. This is a classification task and I will present an algorithm that does just that by beginning with feature selection & extraction, choosing an algorithm or a combination of algorithms through to classification.

## The data

The data, obtained from Kaggle and [Appen](https://appen.com/resources/datasets/) consists of a [training/development set](data/train.csv) and a [test set](data/test.csv) with the following information about a tweet:

- the text of a tweet
- A keyword from that tweet (may be blank)
- the location of the tweet (may be blank)

## Feature Selection

The question is what features of the tweets are important in determining whether a tweet describes an actual disaster or not. At the surface level, we can simply decide to select tweets that mention disaster-related words to be of class **1** but we need to go deeper than that.

## Evaluation

The model will be evaluated using the F1 score against a test set that I have not tuned my model towards, on Kaggle.

## References

1. [Real or Not? NLP with Disaster Tweets. Predict which Tweets are about real disasters and which ones are not](https://www.kaggle.com/c/nlp-getting-started/overview)
