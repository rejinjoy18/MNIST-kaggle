# MNIST-kaggle

mnist_kaggle is the main file to train and test the data. 
Imgaugment contains python code to augment images such as add noise, blur etc. to increase training data size. (source: imgaugment adapted from github user: "codebox". Modified by me according to requirement)
The network is trained with two convolutional layers, two max pooling layers and two fully connected layers. A training data set of 160,000 images is fed into the network after image augmentation including image blur, image transform, image resize, and image noise addition. 
A test set of 10,000 images is used.
