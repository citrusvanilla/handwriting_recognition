# Handwriting Recognition with Deep Learning in TensorFlow

This repository contains a Jupyter notebook that walks the user through a method for recognizing handwriting through classification of the [notMNIST](http://yaroslavvb.blogspot.com/2011/09/notmnist-dataset.html) character dataset.  This dataset is designed to look like the classic [MNIST](http://yann.lecun.com/exdb/mnist/) dataset, while looking a little more like real data: it's a harder task, and the data is a lot less 'clean' than MNIST:

![alt text](http://i.imgur.com/lcyDFO1.png)

A quick and simple two-layer convolutional neural network with max pooling filters and RELU nonlinearily activation functions, followed by one fully-connected layer, is fit to the data. The model obtains a ~8% error rate on a test set after just minutes on a personal CPU.  The model architecture is a simplified variant of the classic [LeNet5](http://yann.lecun.com/exdb/lenet/).  Implementation uses the TensorFlow library.

## Software and Library Requirements
* Python 2.7.11
* Jupyter Notebook 4.2.2
* Numpy 1.11.2
* scikit-image 0.12.3
* TensorFlow 0.17

## Code Organization

File | Purpose
------------ | -------------
handwriting_recognition_data.py | Contains a variety of functions and methods for downloading and preprocessing the dataset.

## Getting up and running

Make sure you are in the top-level project directory `handwriting_recognition/`. Then run:

> ipython notebook handwriting_recognition_walkthrough.ipynb
