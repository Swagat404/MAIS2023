# Overview
This is a kaggle challenge as part of the final assignment for MAIS 2023.
https://www.kaggle.com/competitions/mais-202-winter-2023/overview

# Model Used
I used Gradient Boosting for classifying the images according to the labels. The weights have been saved as a binary file:model1 after training it with the images in the dataset.

# Accuracy achieved
The evaluation metric for this competition is *class label accuracy*.A public score of 0.82 was achieved with the predicted labels

# Submission
submission.csv has the predicted labels which was submitted for this challenge.

# How to use?

```bash

from sklearn.ensemble import GradientBoostingClassifier
from sklearn.datasets import load_iris
from sklearn.metrics import accuracy_score
iris = load_iris()
X, y = iris.data, iris.target
clf = GradientBoostingClassifier(n_estimators=100, learning_rate=0.1, max_depth=3)
```

Load the saved weights from model1 and predict new labels


