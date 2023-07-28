# Apparel-Recommendations
Content Based Filtering and Recommendation
# Amazon Apparel Recommendation System

![Python](https://img.shields.io/badge/Python-3.7%2B-brightgreen.svg) ![Machine Learning](https://img.shields.io/badge/Machine_Learning-Deep_Learning-blue.svg) ![Image Processing](https://img.shields.io/badge/Image_Processing-NLP-orange.svg) ![Recommendation System](https://img.shields.io/badge/Recommendation_System-Content_Based_Filtering-yellow.svg)

# Amazon Apparel Recommendation Engine

## Overview

This project implements a personalized apparel recommendation engine using content-based search with the Amazon API, NLTK, and Keras libraries. It involves processing over 180,000 apparel images from a JSON file for recommendation. Seven different approaches are utilized to recommend apparel, including Bag of Words, TF-IDF, Word2Vec, IDF, weighted Word2Vec, weighted similarity using brand and color, and visual features using Convolutional Neural Networks (CNN). The models are trained using GPU for efficient computation.

## Implementation Steps

1. Data Preprocessing: The JSON file containing apparel images is extracted and preprocessed to ensure data quality. Irrelevant coordinates and trip details are removed, and data is prepared for clustering and segmentation.

2. Clustering and Segmentation: The whole dataset is divided into clusters/segments/regions using K-Means clustering algorithm. Cluster numbers are assigned to each data point based on pickup coordinates.

3. Time-Binning and Fourier Transform: Time-series data is analyzed using Fourier transform to identify significant amplitudes and frequencies. The data is then divided into 10-minute time bins for better predictions.

4. Model Selection and Training: Seven different models, including Bag of Words, TF-IDF, Word2Vec, IDF, weighted Word2Vec, weighted similarity, and CNN, are implemented and trained on the preprocessed data using GPU.

5. Evaluation and Comparison: The performance of each model is evaluated by calculating the average Euclidean distance for the top 20 recommended apparels. The results are compared using line plots and bar graphs to identify the best performing approaches.

## Observations

- The TF-IDF model exhibits the best recommendation performance, followed by AVERAGE WORD2VEC, BAG OF WORDS, BRAND AND COLOR, WEIGHTED WORD2VEC, IDF, and CNN, respectively.
- The GPU-accelerated training of Word2Vec and CNN models ensures efficient computation and faster results.
- The evaluation metrics indicate that the personalized recommendation engine provides accurate suggestions to users based on their preferences and product attributes.
- The visual features extracted using CNN play a crucial role in improving the accuracy of recommendations for apparel products.

## Conclusion

The personalized apparel recommendation engine showcases the superiority of content-based search methodologies and deep learning techniques. The implementation of various models and their evaluations through quantitative analysis ensures optimal results for end-users. The project demonstrates the efficiency of GPU-accelerated models for faster computation and improved recommendation accuracy.

Feel free to explore the code and findings in the Jupyter Notebook provided in this repository. Your feedback and contributions are welcome! Happy recommending!
