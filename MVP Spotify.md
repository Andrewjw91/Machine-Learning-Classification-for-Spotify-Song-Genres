## MVP: Classification of Spotify Song Genres

![confusion%20matrix.JPG](attachment:confusion%20matrix.JPG)

The above confusion matrix visualizes the results from my Random Forest classification model.
I narrowed down and cleaned my dataset to ~25,000 rows and 12 feature columns, with the 9 genres shown above. 

So far I've run a KNN model and a Random Forest model on my Spotify song dataset. 

With KNN as my baseline, I got an accuracy score of 0.815 on the validation set and 0.835 on the test set.
I then ran KNN with cross validation and got mean accuracy score of 0.825

The Random Forest model significantly outperformed the KNN models and produced the following results:

Test Set Accuracy =  0.92
Test Set F-score =  0.85
ROC AUC = 0.986

As of now, Random Forest is the preferred model. I will try implementing LogisticRegression and XGBoost and compare the model performance/metrics.

The business application of this type of model can benefit Spotify's recommendation algorithm and/or auto-generated playlist algorithm. This model can classify a song to a group label with other songs of similar sonic qualities. Even for the songs that got classified as a false positive, the recommender can still introduce songs from other genres that they might enjoy.


```python

```
