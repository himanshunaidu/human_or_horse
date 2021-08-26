# human_or_horse

Convolutional Neural Network that differentiates between human and horse

## Dataset

Training Set: https://storage.googleapis.com/laurencemoroney-blog.appspot.com/horse-or-human.zip
Validation Set: https://storage.googleapis.com/laurencemoroney-blog.appspot.com/validation-horse-or-human.zip

## Dataset Preprocessing

Scaled by 1/255

## Dataset Extraction Method

Used zipfile python module for zip extraction
Used ImageDataGenerator (from tensorflow.keras.preprocessing.image) for supplying images to neural network

## Convolutional Neural Network

Convolutional Part: 3 Conv2D layers, each followed by a BatchNormalization layer and MaxPool2D layer
  Activation: LeakyRelu with alpha=0.15
  Padding: Valid
  Max-Pooling Stride: 2X2

Dense Part: 2 Dense layers, each followed by a Dropout, and finally a Dense output layer
  Activation: LeakyRelu with alpha=0.15
  Dropout Rate: 0.3
  Output Function: Sigmoid

## Compilation

Optimizer: Adam
Loss Function: Binary Cross-Entropy

## Training

Trained for 15 epochs.
Resultant model overfitted over training data, thus failing in validation accuracy
