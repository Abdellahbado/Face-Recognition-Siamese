# Face Recognition using Siamese Method

## Introduction
This GitHub repository contains code for face recognition using the Siamese method with TensorFlow and Keras. The Siamese method is a technique for training neural networks to recognize and differentiate between pairs of input data. In this case, the goal is to recognize and verify faces.

Please note that the training of this model was not completed due to time and computing constraints. However, the code provides a foundation for implementing the Siamese method for face recognition, and you can further train the model as needed.

## Dataset
The dataset used for this project can be found on Kaggle in the "lfw-deepfunneled" directory. Due to the large size of the dataset, only a subset is used for training and validation.

## Dependencies
- TensorFlow 2.x
- Keras
- NumPy

## Environment
The code may produce some warnings related to TensorFlow optimization and GPU capabilities. If you encounter any issues, consider adjusting the TensorFlow environment variables.

## Code Overview
The code is organized as follows:

1. Importing necessary libraries and setting up TensorFlow environment.
2. Loading the dataset using `tf.keras.utils.image_dataset_from_directory`.
3. Creating a Siamese neural network model with a specified architecture.
4. Generating image pairs and labels for training.
5. Compiling and training the Siamese model.
6. Evaluating the model on the test dataset.

## Model Architecture
The Siamese neural network consists of two identical subnetworks that share the same weights. The distance between the output features of these subnetworks is calculated, and a final decision is made using a binary classification layer.

## Usage
To use this code:

1. Download the "lfw-deepfunneled" dataset from Kaggle.
2. Set the `dataset_dir` variable to the path of the downloaded dataset.
3. Run the code to train the Siamese model.

## Important Note
Please be aware that the training was not completed, and you may need to adjust hyperparameters, training duration, or use more powerful computing resources to achieve desired performance.

Feel free to contribute, enhance, or adapt the code according to your specific requirements. If you encounter any issues or have questions, please open an issue in the GitHub repository.
