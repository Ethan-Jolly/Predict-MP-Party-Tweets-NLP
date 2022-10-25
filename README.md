# Predict-MP-Party-Tweets-NLP

Predicting British MP's political parties using NLP techniques to extract information from their tweets, using a corpus of 74,000 tweets collected using twitters API. In the notebook I compare between 4 different Machine Learning Classifiers as training models, as well as changing different pre-precessing tokenisers and word inclusions. These different classifiers being Random Forest, K Nearest Neighbour, Naive Bayes and Logistic Regression.


## Accuracy Results


<img src="https://user-images.githubusercontent.com/113981071/197834364-4313d495-e372-42b6-9384-e06051e90bf8.png" alt="graphs" width="850"/>

## Looking For Outlier MPs

An additional task I tak in this notebook was to attempt to look for any outlier MPs from either of the parties, to do this I take the best model from the previous results then perform a leave-one out cross-validation, where each model from the cross-validation is training on information from all other MPs. This ensures that for predicting each MP, the models have the most possible information about the two parties.


![heatmapImproved](https://user-images.githubusercontent.com/113981071/197836228-8ddda880-a09b-428e-b3c9-e7857d4e785e.png)

Where the top row are Labor MPs, the bottom row are conservative MPs and the more red in the plot the more the model predicts Labour, the more blue the more it predicts conservative. 
