# human_or_horse
Convolutional Neural Network that differentiates between human and horse

#Dataset
Training Set: https://storage.googleapis.com/laurencemoroney-blog.appspot.com/horse-or-human.zip
Validation Set: https://storage.googleapis.com/laurencemoroney-blog.appspot.com/validation-horse-or-human.zip

#Dataset Preprocessing
Scaled by 1/255

#Dataset Extraction Method
Used zipfile python module for zip extraction
Used ImageDataGenerator (from tensorflow.keras.preprocessing.image) for supplying images to neural network
