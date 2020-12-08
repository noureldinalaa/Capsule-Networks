[//]: # (Image References)

[image1]: ./images/recon.png "Reconstracted image"
[image2]: ./images/encoder_architecture.png "Encoder"

# Capsule-Networks
In this repository I will Simply explain and implement Capsule Networks on MNIST dataset using Pytorch.


## what are capsules?

* Briefly explaining it, capsules are small group of neurons where each neuron in a capsule represents various properties of a particular image part.
* Capsules represent relationships between parts of a whole object by using **dynamic routing** to weight the connections between one layer of capsules and the next and creating strong connections between spatially-related object parts, will be discussed later in the notebook or my bolg post

* The output of each capsule is a vector, this vector has a magnitude and orientation.
    * Magnitude : It is an indicates if that particular part of image is present or not. Basically we can summerize it as the probability of the part existance (It has to be between 0 and 1). 
    
    * Oriantation : It changes if one of the properties of that particular image has changed.


## Model Architecture

The capsule network is consisting of two main parts:

* A convolutional encoder.
* A fully connected, linear decoder.

![Encoder][image2]


## Reconstracted output on test data

![Reconstracted image][image1]





