# Apparel Recommendation System : Content Based Filtering and Recommendation System

## Apparel Recommendation System using featurization techniques and CNN

![Python](https://img.shields.io/badge/Python-3.7%2B-brightgreen?style=for-the-badge&logo=python) ![Machine Learning](https://img.shields.io/badge/Machine_Learning-Deep_Learning-blue?style=for-the-badge) ![Image Processing](https://img.shields.io/badge/Image_Processing-NLP-orange?style=for-the-badge) ![Recommendation System](https://img.shields.io/badge/Recommendation_System-Content_Based_Filtering-yellow?style=for-the-badge) ![VGG-16](https://img.shields.io/badge/Model-VGG--16-blue?style=for-the-badge&logo=python)

## Apparel Recommendation System to enhance Sales

### Overview

This project implements a personalized apparel recommendation engine using content-based search with the Amazon API, NLTK, and Keras libraries. It involves processing over 180,000 apparel images from a JSON file for recommendation. Seven different approaches are utilized to recommend apparel, including Bag of Words, TF-IDF, Word2Vec, IDF, weighted Word2Vec, weighted similarity using brand and color, and visual features using Convolutional Neural Networks (CNN). The models are trained using GPU for efficient computation.

### Implementation Steps

1. <b>Data Preprocessing:</b> The JSON file containing apparel images is extracted and preprocessed to ensure data quality. Irrelevant coordinates and trip details are removed, and data is prepared for clustering and segmentation.

2. <b>Clustering and Segmentation:</b> The whole dataset is divided into clusters/segments/regions using K-Means clustering algorithm. Cluster numbers are assigned to each data point based on pickup coordinates.

3. <b>Time-Binning and Fourier Transform:</b> Time-series data is analyzed using Fourier transform to identify significant amplitudes and frequencies. The data is then divided into 10-minute time bins for better predictions.

4. <b>Model Selection and Training:</b> Seven different models, including Bag of Words, TF-IDF, Word2Vec, IDF, weighted Word2Vec, weighted similarity, and VGG-16 CNN, are implemented and trained on the preprocessed data using GPU.

5. <b>Evaluation and Comparison:</b> The performance of each model is evaluated by calculating the average Euclidean distance for the top 20 recommended apparels. The results are compared using line plots and bar graphs to identify the best performing approaches.

### Observations

- The TF-IDF model exhibits the best recommendation performance, followed by AVERAGE WORD2VEC, BAG OF WORDS, BRAND AND COLOR, WEIGHTED WORD2VEC, IDF, and CNN, respectively.
- The GPU-accelerated training of Word2Vec and CNN models ensures efficient computation and faster results.
- The evaluation metrics indicate that the personalized recommendation engine provides accurate suggestions to users based on their preferences and product attributes.
- The visual features extracted using CNN play a crucial role in improving the accuracy of recommendations for apparel products.

### Conclusion

This personalized apparel recommendation engine showcases the superiority of content-based search methodologies and deep learning techniques. The implementation of various models and their evaluations through quantitative analysis ensures optimal results for end-users. The project demonstrates the efficiency of GPU-accelerated models for faster computation and improved recommendation accuracy.

Feel free to explore the code and findings in the Jupyter Notebook provided in this repository. Your feedback and contributions are welcome! Happy recommending!
