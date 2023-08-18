# TextClassification
**QUALITY CLASSIFICATION OF QUESTIONS ON STACK OVERFLOW**

## Abstract
Community Question Answering (CQA) is the field of computational linguistics that deals with problems derived from the questions and answers posted to websites and it has a growing popularity as a way of providing and researching information. Crowdsourced knowledge is a resource for users yet it can raise concerns about the quality of the shared content. As recognizing good questions that can improve the CQA services and the user’s experience, the study focuses on question quality instead. Using a dataset of questions and answers posted to the Stack Overflow website, we have analyzed and conducted quality classification of questions. In addition to taking advantage of the natural language processing capabilities of neural network Deep Learning models such as LSTM, Bi-LSTM, and Distil-BERT, we also apply some Machine Learning classification models like Logistic Regression, Multinomial Na ̈ıve Bayes, Decision Tree, Random Forest. Then we compare all the models and give the best model to help classify the quality of the question. Initially, the result was obtained with the Distil-BERT model with the highest accuracy of 91.80%.


## Deep learning and machine learning methods
- Deep learning: LSTM, Bi-LSTM, and Distil-BERT.
- Machine learning: Logistic Regression, Multinomial Naıve Bayes, Decision Tree, Random Forest.


## Dataset
[Dataset trên Kaggle](https://www.kaggle.com/datasets/imoore/60k-stack-overflow-questions-with-quality-rate)

The dataset consists of over 60,000 data samples that are collected from the Stack Overflow website. These questions were asked in a time period ranging from January 1st, 2016 to January 1st, 2020. The dataset includes 2 data files: train.csv (45,000 samples), and valid.csv (15,000 samples). The dataset consists of 6 features: a unique question ID, a question title, the main body or content of the question, tags representing the important words (keywords) in the question, the creation date of the question as well as the class/label of the question. The label itself consists of 3 classes:
• **High-Quality (HQ)**: questions that receive a score a more than 30 from the community and is not edited a single time by anyone.
• **Low-Quality Edited (LQ EDIT)**: questions that receive a negative score and multiple edits from the community.
• **Low-Quality Closed (LQ CLOSE)**: questions that were immediately closed by the community due to its extremely poor quality. These questions are sorted according to their question ID. Also, the main content or text of the questions are in the HTML format and the dates are in the UTC format.
