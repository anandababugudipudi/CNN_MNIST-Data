# Convolutional Neural Network Implementation on MNIST Hand Written Digits Data

MNIST (Modified National Institute of Standards and Technology) is the de facto “Hello World” dataset of Computer Vision. It was released in 1999. And from then onwards, this classic dataset of handwritten images has served as the basis for benchmarking classification algorithms. As new machine learning techniques emerge, MNIST remains a reliable resource for researchers and learners alike. In this project, our goal is to correctly identify digits from a dataset of tens of thousands of handwritten images. 

[](https://github.com/anandababugudipudi/CNN_MNIST-Data/blob/main/images/CNN%20MNIST.jpeg)

Image [Source](https://miro.medium.com/max/3288/1*uAeANQIOQPqWZnnuH-VEyw.jpeg)

In this project, we are going to implement the following steps:
1. Importing the necessary packages
2. Loading the MNIST Dataset from Keras Datasets
3. Normalizing the Images
4. OneHot Encoding of output Classes
5. Creating the Convolutional Neural Network
6. Compiling the model
7. Data Augmentation to reduce overfitting
8. Training the model
9. Evaluating the model
10. Making some predictions on model


A **Convolutional Neural Network (ConvNet/CNN)** is a Deep Learning algorithm which can take in an input image, assign importance (learnable weights and biases) to various aspects/objects in the image and be able to differentiate one from the other. The pre-processing required in a ConvNet is much lower as compared to other classification algorithms. While in primitive methods filters are hand-engineered, with enough training, ConvNets have the ability to learn these filters/characteristics.

The architecture of a ConvNet is analogous to that of the connectivity pattern of Neurons in the Human Brain and was inspired by the organization of the Visual Cortex. Individual neurons respond to stimuli only in a restricted region of the visual field known as the Receptive Field. A collection of such fields overlap to cover the entire visual area.

Input is 28 X 28 pixel image with 32 filters in (3, 3) size filter.

`BatchNormalization()` normalizes the activations in the previous layer after the convolutional phase and the tranformation maintains the mean activation close to 0 and standard deviation close to 1. With this the scale of the dimension remains the same, but reduces the running-time of training significantly. 
