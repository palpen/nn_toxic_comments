# Feed-forward Neural Networks and Toxic Comment Classification

This repository contains my experiments on toxic comment classification using feed-forward neural networks implemented in Keras (a TensorFlow API). The data comes from a Kaggle competition that I'm currently participating in ([see here](https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge)). The challenge is a multiclass, multilabel classification of text across various categories of comment toxicity (toxic, severely toxic, obscene, threat, insult, and identity hate).

I trained the model on a GPU which significantly improved training time. I also experimented with dropout regularization to minimize overfitting and improve performance on the test set. The final model improved on a naive baseline (a simple columnwise mean of each category) by 50%.

This is also the project I submitted for my application to [SharpestMinds](https://www.sharpestminds.com/).

The relevant files in this folder are
1. [environment.yml](https://github.com/palpen/sharpestminds/blob/master/environment.yml): Packages used in the project
2. [kaggle_toxic_comment_deeplearning.ipynb](https://github.com/palpen/sharpestminds/blob/master/kaggle_toxic_comment_deeplearning.ipynb): the main Jupyter notebook containing the analysis
3. `train.csv`: the labeled data for training
