# MNIST-kaggle

mnist_kaggle is the main file to train and test the data. 

Imgaugment contains python code to augment images such as add noise, blur etc. to increase training data size. (source: imgaugment adapted from github user: "codebox". Modified by me according to requirement)

The network is trained with two convolutional layers, two max pooling layers and two fully connected layers. A training data set of 160,000 images is fed into the network after image augmentation including image blur, image transform, image resize, and image noise addition. 

A test set of 10,000 images is used and the result is saved onto a csv file for submission to Kaggle.
Dropout is also employed in the problem to reudce overfitting of the data. 

The labels for the training data are converted to one hot vectors for better results and function mini_batch generates random batches of batch_size which is fed in an epoch.
The convolutional layers are initialized as random normal variables with a standard deviation of 0.1 and have a stride of 1. The pooling used is max_pool and has a window and stride size of 2x2.
