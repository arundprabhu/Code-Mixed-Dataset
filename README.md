# Code-Mixed-Dialog

This repository contains the dataset used in our paper : Codeswitched Sentence Creation using Dependency Parsing. 

The sentiment data for Hindi and Marathi are provided in the respective directories. 
We use the code provided in [Sub-word-LSTM](https://github.com/drimpossible/Sub-word-LSTM) for training and testing.

## Method Overview

Given a sentence we extract independent phrases using [Stanford Parser](http://nlp.stanford.edu:8080/parser/). The independent phrases are translated using Google's On-device NMT and transliterated using [Indic trans](https://github.com/libindic/indic-trans). The original phrases are replaced by these phrases in such a way that the CMI of the resulting codemixed sentence is maximum. 

## Dataset generation

We use the test set of [Sentiment 140](http://help.sentiment140.com/for-students) as the original dataset for generating the codemixed dataset. 
