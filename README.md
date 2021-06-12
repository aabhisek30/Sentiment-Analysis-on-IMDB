# Sentiment-Analysis-on-IMDB
Here I have done comparative analysis of SVM, Naive Bayes and LSTM for sentiment analysis


## Libaries and Dataset

1. Pandas
2. Numpy
3. Re
4. Beautiful shop
5. OS
6. Pillow
7. Matplotlib
8. Keras
9. Tensorflow
10. Sklearn
11. Dataset - IMDB Dataset of 50K Movie Reviews (https://www.kaggle.com/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews)

## File 1 - Preprocessing.ipynb

1. Word cloud of review before preprocessing

![Reviews_before_preprocessing](https://user-images.githubusercontent.com/67454437/121723333-03dc2980-cb04-11eb-99a8-ddc5be22fd2d.png)

2. Word cloud of review after preprocessing

![Reviews_after_preprocessing](https://user-images.githubusercontent.com/67454437/121723382-122a4580-cb04-11eb-985a-c9810d1bf7d5.png)

3. We can see that HTML tags like br are removed in the preprocessing stage
4. At the end preprocessed data is saved as preprocessed_dataset.csv

## File 2 - SVM NB.ipynb

1. I have used 2 Text vectorization techinques - BOW and TFIDF
2. I have used Multinoimal Naive Bayes, Bernouli Naive Bayes , SVM with rbf kernel for each word vectorization techniques
3. I have used Hyperparamter tuning to increase the performance of above algorithm


### Without Hyperparamter tuning

| Algorithm      | vectorization | Accuracy |
|:---------------|:--------------|----------| 
| Multinoimal NB | BOW           | 86.34%   |
| Multinoimal NB | TFIDF         | 89.10%   |
| Bernouli NB    | BOW           | 85.78%   |
| Bernouli NB    | TFIDF         | 88.62%   |
| SVM            | BOW           | 88.28%   |
| SVM            | TFIDF         | 90.84%   |

### With Hyperparamter tuning

| Algorithm      | vectorization | Accuracy |
|:---------------|:--------------|----------| 
| Multinoimal NB | BOW           | 86.38%   |
| Multinoimal NB | TFIDF         | 89.10%   |
| Bernouli NB    | BOW           | 85.68%   |
| Bernouli NB    | TFIDF         | 88.62%   |
| SVM            | BOW           | 88.60%   |
| SVM            | TFIDF         | 91.26%   |

## File 3 - LSTM.ipynb

1. Model summary

![image](https://user-images.githubusercontent.com/67454437/121725720-42271800-cb07-11eb-94a3-208467821104.png)

![image](https://user-images.githubusercontent.com/67454437/121725838-64b93100-cb07-11eb-9a78-55a4e14dab97.png)

2. Model is clearly overfitting 

3. Accuracy on Test data - 85.96

4. In order to stop model from overfitting, I used concept of EarlyStopping from Keras

5. Accuracy on Test data - 86.46










