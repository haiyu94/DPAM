# DPAM
code for Modeling Dynamic Pairwise Attention for Crime Classification over Legal Articles [[pdf]](https://dl.acm.org/citation.cfm?doid=3209978.3210057)

## Description
In juridical field, judges usually need to consult several relevant cases to determine the specific articles that the evidence violated, which is a task that is time consuming and needs
extensive professional knowledge. we treat the evidences as documents, and articles as labels, thus
the conviction process can be cast as a multi-label classification problem.

DPAM model is used to predict articles by the evidences. This model adopt the multi-task learning method to learn the multi-label classifier and the threshold predictor jointly.

## Getting Started
1. clone the code
2. download the dataset
3. mv the dataset file into code dir
4. run the script: run.sh

## Working with the code
To work with the DPAM, you can simply run the script: run.sh. and you can also modify the parameters in the DPAM_train.py, then run the script: python DPAM_train.py

## Download
The dataset contains 4 files: one_hot_vocab_70.txt  src_rule_data.txt  src_train_dev_data.txt  stop_words.txt

the download url: https://drive.google.com/open?id=1TCcTzte2cQ2wxWw-kXsZdUApCsNejdn8
### one_hot_vocab_70.txt
this file contains the mapping of the top 70 (labels)articles to one hot representation.
### src_rule_data.txt
the file has two columns, the first column is article number, the second column is labels(articles) description.
### src_train_dev_data.txt
this file contains 17160 samples, which is the train and dev source data, the file has two columns, the first column is evidence description, the second column is labels(articles).
### stop_words.txt
this file contains some stop words, which is ignored in our train and dev samples.
