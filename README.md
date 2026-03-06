# Spice-classification-project

Project Explanation

This project demonstrates how to build and train a Convolutional Neural Network (CNN) using TensorFlow/Keras to classify different types of spices from images.

Key Steps Involved:

Setup and Imports: Imports necessary libraries like TensorFlow, Keras, NumPy, Pandas, Matplotlib, and PIL for image processing.
Dataset Preparation:
Mounts Google Drive to access the dataset.
Defines and verifies the dataset directory structure, expecting subdirectories for each spice class.
Loads image data efficiently using keras.utils.image_dataset_from_directory, which handles resizing, batching, and splitting data into training and validation sets.

Model Building:
Constructs a sequential CNN model with multiple Conv2D, MaxPooling2D, Flatten, and Dense layers.
Includes a Rescaling layer to normalize pixel values.
Compiles the model using SparseCategoricalCrossentropy as the loss function, Adam optimizer, and accuracy as a metric.

Model Training:
Trains the CNN model on the prepared training data, with performance monitored on the validation data over several epochs.
Visualization of Training History:
Plots the training and validation loss and accuracy curves to assess model performance and detect potential overfitting or underfitting.

Model Evaluation:
Evaluates the trained model on the validation set to obtain overall loss and accuracy.
Generates a detailed classification report and a confusion matrix to understand per-class performance, precision, recall, and F1-score.

Prediction Visualization:
Visualizes a sample of random images from the validation set along with their true labels and the model's predictions, highlighting correct and incorrect classifications.

Single Image Prediction:
Provides functionality to upload a single image and have the trained model predict its spice class with a confidence score.
This project serves as a comprehensive example of an image classification workflow using deep learning, from data loading to model deployment for inference on new images.

