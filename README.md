# COVID-19-Healthcare-Misinformation

## Background and Model usage
As the coronavirus spreads, misinformation related to COVID-19 also spreads. Such information has caused confusion among people, disruptions in society, and bad consequences. So the goal is to understand, detect and mitigate the fake news.

## Dataset
- 5,975 confirmed fake and true news articles with ground truth label
- 15.95% news are fake

## Modeling process
- Combine files and create labels
- Create TFIDF
- Stratified train/test split
- Apply sampling methods to train dataset
- Train models on training dataset
- Evaluate models on testing dataset

## Sampling methods:
- Simple oversampling: just duplicates examples in the minority class, and these examples don’t add any new information to the model
- SMOTE: synthesizes new examples for the minority class
SMOTE improves 18.9% relatively on Recall

## Evaluation methods:
Recall: The proportion of actual positives was identified correctly.

## Model performance:
Gradient Boosting Machines with grid search yields the best performance (Recall: 0.705).

