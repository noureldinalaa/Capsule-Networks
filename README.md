[//]: # (Image References)

[image1]: ./images/recon.png "Reconstracted image"
[image2]: ./images/encoder_architecture.png "Encoder"

# Capsule-Networks
In this repository I will simply explain and implement Capsule Networks on MNIST dataset using Pytorch.
For more explanation please check [my blog post](https://noureldinalaa.github.io/capsuleNetwork/) 


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


## Reconstructed output on test dataset

![Reconstracted image][image1]



## Project Instructions

### Instructions

1. Clone the repository and navigate to the downloaded folder.
	
	```	
		git clone https://github.com/noureldinalaa/Capsule-Networks/
		cd Capsule-Networks 

2. Install packages like pytorch and torch vision and some pip packages in requirements text file :
	```
		conda install pytorch torchvision -c pytorch
            pip install -r requirements.txt
	```
3. Open a terminal window and navigate to the project folder. Open the notebook and follow the instructions.

	
	```
		jupyter notebook Capsule network.ipynb
	```



## References
1. https://arxiv.org/pdf/1710.09829.pdf
2. https://cezannec.github.io/Capsule_Networks/
3. https://kndrck.co/posts/capsule_networks_explained/
4. https://github.com/cezannec/capsule_net_pytorch/blob/master/Capsule_Network.ipynb
5. https://www.youtube.com/watch?v=1dIEyZuZui0


