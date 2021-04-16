# Challenge 1: The mysterious Machine

Deadline: 16.04. 18:00 

Handed in: 16.04. ~12:00

## Solution

Our solution can be found in [Challenge-1-Notebook.ipynb](Challenge-1-Notebook.ipynb) and the predictions can be found in [ToTheMooners_prediction.csv.](ToTheMooners_prediction.csv)

In the jupyter notebook we documented our process, where we first did some data analysis and data processing on the given training set, explored a simple classifier, compared it to standard classifiers from the scikit learn library and finally defined our classifier as an ensemble model of three of the best classifiers in this comparison with optimized hyperparameters using a cross-validation routine. Last our classifier looks for outliers and predicts those as 0, independently of the ensemble model prediction.

Feedback is highly appreciated!

## Alternative approach

There is a second attempt at the problem using neural networks. In the process of working on the project this idea got discarded due to bad results. Nonetheless feedback is appreciated.

This notebook can be found in [ml_challenge_neural.ipynb.](ml_challenge_neural.ipynb)




