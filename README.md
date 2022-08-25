# Italian-Hate-Speech-Detection
Italian hate speech detection using transformer. We compare monolingual models in both Italian and English (where the Italian dataset is
translated into English) and a multilingual model, and show that the multi-lingual model outperforms monolingual models on this classification task.

## Overview
The University of Bologna (UniBo) Natural Language Processing (NLP) project. In this project, we utilised the PAN-AP-2021 dataset to profile hate speech spreaders on social media, more specifically on Twitter, addressing the problem in English. 

Three different transformers (Italian Transformer, Multilingual transformer, English transformer with translated dataset) were trained and evaluated on the dataset. Our results show that the Multilingual transformer method produces the best results in terms of accuracy on the test set.  

The steps taken are described in detail in the [Report](LINK MISSING). The slides used for the [Presentation](LINK MISSING) are also available.

The code may also be viewed directly from the [Notebook](LINK MISSING).

## Authors
- [Anna Fabris](https://github.com/annafabris)
- [Miki Mizutani](https://github.com/mikimizutani)

## Results
The table below shows the F1-score on the test dataset using the three different transformer.

|     Method     | F1-score hate | F1-score not hate |
|:--------------:|:-------------:|:-------------:|
| Italian transformer   |          41% | 92% |
| Multilingual transformer |          48% | 92% |
| English transformer with translated dataset |  48% | 86% |
