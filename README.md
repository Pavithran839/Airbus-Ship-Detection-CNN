# Airbus-Ship-Detection-CNN
# Airbus Ship Detection Using CNN

## Project Overview

This project uses a Convolutional Neural Network (CNN) to classify satellite images as either containing a ship or containing no ship.

## Objectives

* Build a CNN-based binary image classifier.
* Preprocess and resize satellite images.
* Train and evaluate the model using labelled images.
* Analyze performance using classification metrics and visualizations.

## Dataset

The project uses the Airbus Ship Detection dataset from the Kaggle competition.

Dataset: https://www.kaggle.com/competitions/airbus-ship-detection/data

A balanced subset of 20,000 images was used:

* Training: 14,000 images
* Validation: 3,000 images
* Testing: 3,000 images

The dataset itself is not included in this repository.

## Methodology

1. Load and label the satellite images.
2. Resize images to 128 × 128 pixels and normalize pixel values.
3. Train a CNN with convolution, max-pooling, and dense layers.
4. Use binary cross-entropy loss and the Adam optimizer.
5. Evaluate the model on the held-out test set.

## Results

| Metric        | Result |
| ------------- | -----: |
| Test Accuracy | 88.17% |
| Precision     | 87.64% |
| Recall        | 88.87% |
| F1-score      | 88.25% |
| Test Loss     | 0.2991 |

These results were obtained on the balanced 3,000-image test subset.

## Results and Visualizations

See the `results/` directory for the training and validation graphs, confusion matrix, and final metrics table.

## Technologies Used

* Python
* TensorFlow / Keras
* NumPy and Pandas
* Matplotlib
* Scikit-learn
* Google Colab with GPU acceleration

## How to Run

1. Open the notebook in Google Colab.
2. Obtain access to the Kaggle dataset.
3. Configure Kaggle authentication securely using Colab Secrets.
4. Follow the notebook cells to prepare the data, train the CNN, and evaluate the results.

## Team

Two-person student project.

## License

Dataset usage is subject to the terms of the original Kaggle competition.
