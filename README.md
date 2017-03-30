This repository uses data found on [Kaggle](https://www.kaggle.com/dalpozz/creditcardfraud).

## Conclusion

The dataset was split 70:30 for training and testing.

SMOTE was applied on the training set to establish a 1:1 ratio prior to being given to the models.

Results, (50% threshold where applicable):

| Model         | Accuracy | Precision | Recall | PR-AUC | ROC-AUC |
|---------------|----------|-----------|--------|--------|---------|
| Random Forest | 0.9996   | 0.9352    | 0.8387 | 0.8845 | 0.9818  |
| Neural Net    | 0.9994   | 0.8435    | 0.8000 | 0.8368 | 0.9471  |


The most successful model was a random forest with 128 trees.

However the neural net shows promise. Although it is underperforming our random forest somewhat, much time was spent on optimizing conditions for the random forest.

As a result it is possible the neural net may improve with finer tuning.

In addition, the dataset is still relatively small, so if we were able to get more examples of fraudulent data, it is possible the neural net will be more performant and efficient in the long run.

For now at least, the random forest produces a fairly suitable model at both catching fraudulent transactions while not causing too much annoyance for customers making legitimate transactions.
