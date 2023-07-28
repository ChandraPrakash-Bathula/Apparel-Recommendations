# Apparel-Recommendations
Content Based Filtering and Recommendation
# Amazon Apparel Recommendation System

![Python](https://img.shields.io/badge/Python-3.7%2B-brightgreen.svg) ![Machine Learning](https://img.shields.io/badge/Machine_Learning-Deep_Learning-blue.svg) ![Image Processing](https://img.shields.io/badge/Image_Processing-NLP-orange.svg) ![Recommendation System](https://img.shields.io/badge/Recommendation_System-Content_Based_Filtering-yellow.svg)

## Overview

This project focuses on building a personalized recommendation system for apparel products using content-based filtering. The system recommends similar apparel products based on various attributes such as asin, brand, color, product type, image URL, title, and formatted price. Different techniques, including Bag of Words, TF-IDF, IDF, Word2Vec, IDF Weighted Word2Vec, and Convolutional Neural Networks (CNN), have been utilized to achieve accurate and relevant recommendations.

## Steps Implemented

1. Data Collection: We extracted over 180,000 apparel images and their attributes from the Amazon API to create our dataset.

2. Data Preprocessing: We cleaned and processed the data, removing irrelevant coordinates, trip durations, speeds, and fares to ensure data quality.

3. Clustering/Segmentation: New York City was divided into clusters/segments/regions based on pickup latitudes and longitudes using K-Means clustering.

4. Time-binning: We used Unix timestamps to group the data into 10-minute time intervals for prediction.

5. Smoothing Time-series Data: To avoid predicting zero pickups, we smoothed the training data and filled test data with zeros.

6. Fourier Transform: A Fourier transform was applied to the time-series data to identify top amplitudes and corresponding frequencies.

## Observations

- **TF-IDF Model**: The TF-IDF model emerged as the top-performing approach, providing the most accurate and relevant recommendations.
- **Average Word2Vec Model**: The Average Word2Vec model also performed well, closely following the TF-IDF model in terms of recommendation accuracy.
- **Bag of Words Model**: The Bag of Words model demonstrated a competitive performance, though not as accurate as TF-IDF and Average Word2Vec.
- **Brand and Color Weighted Model**: The model incorporating brand and color as weighted features showcased promising results.
- **IDF Model**: The IDF model, though effective, ranked lower than TF-IDF, Average Word2Vec, and Bag of Words.
- **CNN Model**: The Convolutional Neural Network (CNN) approach for visual feature extraction played a significant role in improving recommendations.

## Conclusion

The apparel recommendation system successfully utilizes various content-based filtering techniques and visual feature extraction using CNN to provide accurate and relevant suggestions to users. The project's observations emphasize the effectiveness of the TF-IDF and Average Word2Vec models, while the inclusion of brand and color as weighted features also contributes to better recommendations. The system's implementation represents a significant step towards creating an engaging and efficient recommendation engine for apparel products.
