# Fake News Detectione with Machine Learning Algorithms and Neural Network Models

## Description

The above project was implemented in the context of the course Text Mining and Natural Language Processing during my postgraduate studies in the Data and Web Science program of the Aristotle University of Thessaloniki.    Its main objective was to compare machine learning algorithms and neural models such as LSTM and Bi-LSTM.

##  Dataset

The dataset is: https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset


## Data Analysis
The initial phase of the analysis involved examining the dataset related to fake and real news. The following visualizations and counts were obtained:

Fake News
The count of subjects in the fake dataset was analyzed, and the results were sorted in descending order. The visualization of fake text data was also conducted.

![image-1](https://user-images.githubusercontent.com/19438003/190975248-54f1f5a7-47c4-48f9-955c-6c326d15b6ee.png)

![image-2](https://user-images.githubusercontent.com/19438003/190975991-9daaeb62-717d-4879-9842-44fdd0b0664f.png)


Real News

The count of subjects in the real dataset was analyzed, and the results were sorted in descending order. The visualization of real text data was also conducted.

![image-3](https://user-images.githubusercontent.com/19438003/190975512-48c20732-9665-4ef0-9bbc-29342c78ab20.png)


![image-4](https://user-images.githubusercontent.com/19438003/190976298-65ffeda3-2476-432f-b009-950c44700294.png)


## Data Preprocessing

To prepare the data for modeling, several preprocessing steps were performed:

The "reuters" or "tweets" information was removed from the text column.
Rows with empty text columns were dropped from the fake/real datasets.
Publisher information was extracted from the text data and saved in a new column.
The title and text columns of the fake/real datasets were merged based on the text column.
The class column was created for both the fake and real datasets.
Special characters like (,.# @) were removed.
Each word was converted into a sequence of 100 vectors.
Each word in the text data was converted into a sequence of numbers (e.g., 1, 2, 3, 4, 5).
The length of each sequence was adjusted to 1000 words.

### Models

LSTM (128 Units)
Bi-LSTM (128 Units)
Gaussian Naive Bayes
Random Forest
Decision Trees
Logistic Regression
Linear Support Vector Machines
K-nearest Neighbors
Ada Boost
XGboost
Voting Classifier (Random Forests, Logistic Regression, KNN)
Voting Classifier (Random Forests, Decision Trees, Gaussian Naive Bayes)

### Evaluation Metrics
Total Training Time
Accuracy, Precision, Recall, F1-Score
Confusion Matrix

### Results

#### Training Time
LSTM and Bi-LSTM models were trained using an RTX 3060 Laptop GPU.

![image-5](https://user-images.githubusercontent.com/19438003/190997141-bd2f0817-8b44-4e6f-9c07-017ffe75ce41.jpg)

#### Scores
![image-6](https://user-images.githubusercontent.com/19438003/190997226-9fd01ebf-f9a6-4ecc-98b2-faa96354bd2a.jpg)


## Conclusions
Based on the results obtained, the following conclusions can be drawn:

The Bidirectional LSTM and LSTM models performed the best among the models tested.
XGBoost also showed decent performance with slightly lower classification accuracy but faster training rates.
