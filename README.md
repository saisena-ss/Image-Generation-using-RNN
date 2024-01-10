# Image-Generation-using-RNN
### Generating Bottom Half of MNIST Digit using RNN

## Overview
This project demonstrates an application of Recurrent Neural Networks (RNNs) to generate the bottom half of MNIST digit images. The model successfully reconstructs the lower portion of handwritten digits using only the upper half as input, showcasing the potential of RNNs in image generation tasks.

## Features
- **Data Preprocessing**: Converts each MNIST image into 7x7 patches, which are then used as sequences for the RNN.
- **RNN with LSTM Layers**: Employs a neural network with 2 LSTM layers, each containing 64 cells, followed by a dense layer for effective sequential data processing.
- **Sequential Image Generation**: The network takes the first 16 patches (top half of the digit) to predict the next 7x7 patch. It then uses a sliding window approach where the last 16 patches (including the newly generated ones) are used for subsequent predictions.

## Dataset
- The project utilizes the MNIST dataset, a large database of handwritten digits commonly used for training and testing in the field of machine learning.
