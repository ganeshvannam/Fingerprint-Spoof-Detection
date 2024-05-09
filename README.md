# Spoof Detection with SVM using HOG and LBP Features

This repository contains Python code for spoof detection using Support Vector Machine (SVM) classifiers trained on Histogram of Oriented Gradients (HOG) and Local Binary Pattern (LBP) features. Spoof detection is a common task in computer vision and security systems to differentiate between real/live images and fake/spoofed images.

## Dataset

The dataset used for training and testing consists of two classes: live images (positive samples) and spoof images (negative samples). The dataset is organized into separate directories for training and testing, with live and spoof images stored as PNG files.

## Code Overview

- `spoof_detection_svm.ipynb`: Jupyter Notebook containing the Python code for spoof detection using SVM classifiers with HOG and LBP features.
- `data/train_live/`: Directory containing live images for training.
- `data/train_spoof/`: Directory containing spoof images for training.
- `data/test_live/`: Directory containing live images for testing.
- `data/test_spoof/`: Directory containing spoof images for testing.

## Feature Extraction

The code extracts either HOG or LBP features from the images based on the chosen feature type. These features are used to train SVM classifiers for spoof detection.

- **HOG Features**: Histogram of Oriented Gradients features capture the local shape and structure of an image by computing gradients and orientations of image patches.
- **LBP Features**: Local Binary Pattern features describe the local texture patterns in an image by comparing each pixel with its neighboring pixels.

## Model Training and Evaluation

The code trains SVM classifiers using the extracted features from the training data. The trained models are then evaluated on the test data to measure their performance in terms of precision, recall, F1-score, and accuracy.

## Usage

1. Ensure you have Python installed, along with the necessary libraries specified in the code.
2. Organize your dataset into directories as described above.
3. Open and run the Jupyter Notebook `spoof_detection_svm.ipynb`.
4. Choose the desired feature type (HOG or LBP) by setting the `feature_type` variable.
5. Execute the code cells to extract features, train SVM models, and evaluate their performance.
6. Review the classification report to assess the performance of the trained models.

## Results

The classification report provides metrics such as precision, recall, F1-score, and accuracy for both classes (live and spoof). These metrics indicate how well the SVM classifiers perform at distinguishing between live and spoof images.

## Note

- Experiment with different parameters for feature extraction and SVM training to optimize model performance.
- Ensure that the dataset is representative and balanced to prevent bias in model training and evaluation.

