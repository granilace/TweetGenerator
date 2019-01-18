# TweetGenerator
Neural network for writing tweets like @realDonaldTrump

This model consists of two networks:
1. [Pre-trained RNN](http://nlp.fast.ai/category/classification.html) on Wikitext-103 and [fine tunned](https://nips2018creativity.github.io/doc/Transfer%20Learning%20for%20Style-Specific%20Text%20Generation.pdf) on last 2.7k tweets from Trump's Twitter loaded via Twitter API
2. 2-layer GRU char-RNN for proper letter capitalization

Some examples of generated tweets:
* I am pleased to announce that I will serve a six - year term at the @whitehouse!
* There is no reason to spend a year without a wall. I want to protect the border and trade, as many as possible. Fix it!
* "You have to take care of yourself. If you don’t, no one else will." – think like a champion
* These are the years of the most angry and dangerous immigration reform.
* The Senate in November is a total mess. They are weak on crime and border security.

more: https://twitter.com/realTrumpIdeas
# Requirements
* fastai>=1.0
* PyTorch>=1.0
* numpy
* pandas
* python-twitter
