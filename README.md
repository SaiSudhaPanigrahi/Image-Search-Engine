# Building Multiple Models For Image Search Engine

## Abstract
This was written for the final project of [Applied Machine Learning Course](https://cornelltech.github.io/cs5785-fall-2018/) conducted at Cornell Tech in Fall 2018. We are promoted to attempt multiple approaches to build a
search engine for searching relevant images given natural
language queries.

The basic understanding is to map textural
information and image representation. Through the process of
processing the data, we had implemented multiple methods in machine learning
including **Bag of Words Model**, **Random Forest Regression**,
**Linear Regression**, **k-Nearest Neighbors Algorithm**, **Principal
Component Analysis**, and **Partial Least Squares Regression**.

Among all the experiments, our highest score on Kaggle is **0.2921**, which ranked 44th of 73 teams. The best approach we achieved uses **Partial Least Square Regression**= on images’ 5 - sentences
descriptions and image features extracted from the intermediate
layer of pre-trained Residual Network.

**[The paper](report.pdf)** discusses each approach and results in details.


## Performance
|                                        Model                                       | Kaggle Score |
|:----------------------------------------------------------------------------------:|:------------:|
|               BoW + LinearRegression + (KNN),(descriptions and tags)               |    0.13968   |
|            BoW + RandomForestRegression + (KNN) (descriptions and tags)            |    0.22065   |
|                        BoW + PCA + RandomForestRegression +                        |    0.09402   |
| BoW + PCA + PartialLeastSquaresRegression,+ (KNN) (Descriptions and pool5 feature) |    0.29212   |

* [Kaggle Competition](https://www.kaggle.com/c/cs5785-fall18-final)
