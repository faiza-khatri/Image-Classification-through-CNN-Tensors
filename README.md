# Image-Classification-through-CNN-Tensors
The project implements a CNN model using a self-designed Tensor ADT.

It takes in image tensors and processes them through a CNN model, using four layers, which are all represented as functions of the Tensor ADT. The images are then classified in binary categories, whether it contains a gun or a knife.

A dataset of 500 images is used for training and forward propagation, with correspnding image label train of binary values, 0 for guns and 1 for knives.

The layers are:
- Convolution : processes and creates the edges, the bias is added to provide variation in the image multiplication reuslts.
- Leaky ReLU : adds non linearity to the data, leaving positive values as is and exponentiating negative values.
- Softmax : exponentially maximizes the difference in values of the images, discretizing the values for prediction set.
- Batch Normalization : repeatdely normalizes all values to make computation easier.

Backward propagation calculates error percenatges and updates accordingly. There are a total of 50 epochs.


