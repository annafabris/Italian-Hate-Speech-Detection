# Italian Hate Speech Detection
Italian hate speech detection using transformer. We compare monolingual models in both Italian and English (where the Italian dataset is
translated into English) and a multilingual model, and show that the multi-lingual model outperforms monolingual models on this classification task.

## Overview
The University of Bologna (UniBo) Natural Language Processing (NLP) elective project work. In this project, we utilised the [Italian Hate Speech Corpus](https://github.com/msang/hate-speech-corpus) dataset to profile hate speech spreaders on social media, more specifically on Twitter, addressing the problem in Italian. 

Three different transformers were trained and evaluated on the dataset. 
- **Italian Transformer**
- **Multilingual transformer**
- **English transformer with translated dataset**

Our results show that the Multilingual transformer method produces the best results in terms of accuracy on the test set.  

The steps taken are described in detail in the [Report](https://github.com/annafabris/Italian-Hate-Speech-Detection/blob/main/Report.pdf). The slides used for the [Presentation](https://github.com/annafabris/Italian-Hate-Speech-Detection/blob/main/Presentation.pdf) are also available.

The code may also be viewed directly from the [Notebook](LINK MISSING).

## Authors
- [Anna Fabris](https://github.com/annafabris)
- [Miki Mizutani](https://github.com/mikimizutani)

## Results
The table below shows the F1-score on the test dataset using the three different transformer.

|     Method     | F1-score hate | F1-score no hate |
|:--------------:|:-------------:|:-------------:|
| Italian transformer   |          31% | 92% |
| Multilingual transformer |          44% | 92% |
| English transformer with translated dataset |  28% | 78% |

The difference between the F1-score of the classes is because the labels the labels are highly unbalanced.
To combat this, weight biasing was tested, however it gave mixed results. While applying a weight bias to the under-represented label (1:2 to no-hate, hate) gave better performance for the hate class, it inhibited the results of the no-hate class. Below is the confusion matrix for the multilingual transformer with a weight bias.
![Alt text](confusion_matrix.png?raw=true)

