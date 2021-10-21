# Sentiment-Analysis " Academic Project "
Building a model that predicts the mean opinion score(MOS) criteria using NLP

# Problems
* Small dataset(151 samples)
* Unbalanced dataset(class number 4 (MOS = 4) has much more values than the others)

![raw data](https://user-images.githubusercontent.com/88405252/138190838-22c51f7e-ae83-4630-8f59-9995c442338b.png)

# Solution ===> Data Augmentation
To augment our text data we will use **nlpaug** which is a library for textual augmentation in machine learning experiments. The goal is improving deep learning model performance by generating textual data.

In this project we will use **nlpaug.augmenter.word.synonym** to replace a few words with their synonyms.

Our data after augmentation: **More samples** & **Balanced**

![data_augmented](https://user-images.githubusercontent.com/88405252/138190856-54527d8f-7df3-4fe7-9e4e-24de886221f3.png)

# Notes
* There are other ways to augment text data using nlpaug like replacing words based on the context using powerful transformer models (BERT).
* We improved the accuracy from 60% ( same model & raw data ) to 72% accuracy after augmenting the data with a few lines of code.
