# Image-Classification-with-Keras
## Problem Statement
The objective of this project is to classify the images using convolutional neural network and optimize the architecture for better accuracy.

## Dataset
The dataset used for this project is CMU face images. This dataset consists of faces of 20 different persons with two different variation combinations in each picture. The two different combinations include orientation(straight, right, left, up, down) and expression(sad, neutral, happy, angry).

## Approach
4kb images were used in the project and these images are read using the NumPy array. A target variable has been created for each of these variables from 1 to 20 and later converted into dummy variables. The dataset is split into train, validation and test for training, hyperparameter tuning and testing respectively. Three different variations of the dataset were created: 1. The original image converted into binary image 2. Sobel filter is applied on the original image so only the contours of the images are visible. 3. The data is normalized. All these variations were used in the training to acheive better accuracy. Two different CNN architectures were build, one using the LeNet architecture and the other architecture is customized to suit the needs of the project. The customized model showed better results than the LeNet model but the number of parameters were more. The model is futhur tuned for batch size, learning rate, activation function, optimizer and kernel initializer.

## Results 
The final model has approximately 2M parameters. This model has tanh as the activation function, SGD optimizer with a learning rate of 0.001 and he uniform kernel initializer. This model has an accuracy of 99 percent.




