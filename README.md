# Toxic-comment-classification
Classification of comments into toxic or non-toxic and additional toxicity subtype attributes like identity attack, threat, insult, etc.

# Description
The dataset contains text comments collected from social media posts and, the target toxicity and additional toxicity subtype attributes which are rated as continuous values between 0 and 1. The dataset contains around 18 lakh data points and around 4 lakh data points were used to perform the model training and one lakh data points were used to test the models.
- The dataset used for the project can be found [here](https://www.kaggle.com/fedesoriano/traffic-prediction-dataset).

# Getting started
## Dependencies 
- `Pandas`
- `Numpy`
- `Matplotlib`
- `Seaborn`
- `Sklearn`
- `Pickle`
- `NLTK`
- `Wordcloud`

## Machine learning Classifiers 
 **Multinomial Naive Bayes**
 
 
In Natural Language Processing(NLP), the Multinomial Naive Bayes method is a common Bayesian learning approach. Using the Bayes theorem, the program estimates the tag of a text, such as an email or a newspaper piece. It assesses the likelihood of each tag for a given sample and returns the tag with the highest probability. The Naive Bayes classifier is made up of several algorithms, all of which have one thing in common, each feature being classified is unrelated to any other feature. The presence or absence of one trait has no bearing on the inclusion or exclusion of another.  An accuracy of 92.49% was secured using this model.

**Linear SVC**

The Linear Support Vector Classifier (SVC) approach uses a linear kernel function to classify data and works well with huge datasets. When compared to the SVC model, the Linear SVC adds additional parameters such as penalty 1(i.e., C=1), normalization (L1 or L2), and loss function. It is designed to fit to the data you provide and provide a ”best fit” hyperplane that divides or categorizes your data. Following that, you may input some features to your classifier to check what the ”predicted” class is after you’ve obtained the hyperplane, securing an accuracy of 94.82% by using this model.

**XGBoost Classifier**

It is an ensemble learning technique that builds a strong classifier by combining different weak classifiers. At first, a model is built using training data, and the second model is built in a way that it tries to correct the misclassification done in the first and this keeps on repeating till the training data is correctly classified or till a maximum number of models is reached.XGBoost classifier was used to train the model and the model was evaluated, securing an accuracy of 93.72% using this model.

**Logistic Regression**

Logistic Regression is a classification system based on Machine Learning. It’s a method for predicting a categorical dependent variable from a set of independent variables. The solver used was “sag” as it performs well when there is a large dataset and the cost function used was the “sigmoid function” which converts the predicted values into the probabilities between the range 0 and 1, securing an accuracy of 94.41% using this model.

## Comparision of Classifiers
We have compared the four different Machine Learning models (Random forest, Linear SVC, MULTINOMIAL Naive Bayes,
XG Boost). For these models, along with accuracy, measures like precision, recall, and F1-score were compared.

## References
- [Ref 1](https://github.com/jayspeidell/ToxicCommentClassification-/blob/master/ToxicComments_EDA.ipynb)
- [Ref 2](https://www.analyticsvidhya.com/blog/2021/12/different-methods-for-calculating-sentiment-score-of-text/)
- [Ref 3](https://saejournal.com/wp-content/uploads/2021/07/Personality-Prediction-Using-Machine-Learning.pdf)
- [Ref 4](http://scikit-learn.org/stable/modules/generated/sklearn.naive)



