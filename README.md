# Image-Recognition-binary-classification-byCNN
Use convolutional neural networks (CNNs) with complex images: 
Building a horses-or-humans classifier that will tell if a given image contains a horse or a human, where the network is trained to recognize features that determine which is which. 
The training set is the data that is used to tell the neural network model that "this is what a horse looks like" and "this is what a human looks like."
Here, I displayed a batch of eight horse pictures and eight human pictures.
Note that because it is a binary classification problem, needed to be ended the CNN with a sigmoid activation so that the output of network will be a single scalar between 0 and 1, encoding the probability that the current image is class 1 (as opposed to class 0).
Data that goes into neural networks should usually be normalized in some way to make it more amenable to processing by the network. (It's uncommon to feed raw pixels into a CNN.) In this case, I preprocessed my images by normalizing the pixel values to be in the [0, 1] range (originally all values are in the [0, 255] range).
Picked a random image from the training set, then generate a figure where each row is the output of a layer and each image in the row is a specific filter in that output feature map. Rerun that cell to generate intermediate representations for a variety of training images.
From the raw pixels of the images to increasingly abstract and compact representations. The representations downstream start highlighting what the network pays attention to, and they show fewer and fewer features being "activated." Most are set to zero. That's called sparsity. Representation sparsity is a key feature of deep learning.
Those representations carry increasingly less information about the original pixels of the image, but increasingly refined information about the class of the image.
