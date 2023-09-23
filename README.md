# Anomaly-Detection

This GitHub repository contains a comprehensive anomaly detection project that includes data preparation, training various recurrent neural network (RNN) models, handling unbalanced data, and using statistical methods for anomaly detection. The project is designed to help you detect anomalies in time-series data efficiently.

## Table of Contents

1. [Introduction](#introduction)
2. [Data Preparation](#data-preparation)
3. [Creating and Training RNN Models](#creating-and-training-rnn-models)
4. [Preprocessing Data for Improved Performance](#preprocessing-data-for-improved-performance)
5. [Training a Self-Supervised Model](#training-a-self-supervised-model)
6. [Handling Unbalanced Data](#handling-unbalanced-data)
7. [Statistical Anomaly Detection](#statistical-anomaly-detection)
8. [License](#license)
9. [Conclusion](#conclusion)

## Introduction<a name="introduction"></a>

Anomaly detection is a critical task in various domains, including finance, cybersecurity, and industrial operations. This project aims to provide a comprehensive solution for anomaly detection in time-series data.

## Data Preparation<a name="data-preparation"></a>

In this section, I prepare the data for training and testing. The data is loaded from CSV files, and a random selection of five datasets is visualized using charts.

## Creating and Training RNN Models<a name="creating-and-training-rnn-models"></a>

I create and train three different RNN models: SimpleRNN, LSTM, and GRU. These models are designed to learn patterns in the time-series data that can help identify anomalies.

## Preprocessing Data for Improved Performance<a name="preprocessing-data-for-improved-performance"></a>

To enhance the performance of the models, I apply two preprocessing methods to the data:

1. **MinMaxScaler**: I scale the data to a specified range to improve convergence during training.
2. **Normalization using L2 norm**: I normalize the data using the L2 norm to make the models more robust to variations in scale.

I then retrain the RNN models with the preprocessed data.

## Training a Self-Supervised Model<a name="training-a-self-supervised-model"></a>

In this section, I train a self-supervised model that uses an LSTM layer. The model is initially trained to predict the next value in the time series. I then remove the last layer of the model and add two dense layers. Finally, I fine-tune the model for anomaly detection.

## Handling Unbalanced Data<a name="handling-unbalanced-data"></a>

Imbalanced data is a common challenge in anomaly detection. I address this issue by downsampling the majority class to balance the dataset. This balanced dataset is used to train a GRU model for anomaly detection.

## Statistical Anomaly Detection<a name="statistical-anomaly-detection"></a>

In this section, I employ statistical methods to detect anomalies in the time-series data. I calculate Z-scores for each data point and use a predefined threshold to classify anomalies.

## License<a name="license"></a>

This project is licensed under the [MIT License](LICENSE).

## Conclusion<a name="conclusion"></a>

This project provides a comprehensive approach to anomaly detection in time-series data, combining machine learning models, data preprocessing, and statistical methods. By following the steps outlined in this repository, you can effectively detect anomalies in your own time-series datasets.

If you have any questions or suggestions, please feel free to reach out and contribute to this project. Your feedback is valuable!

