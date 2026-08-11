- Convolutional Neural Networks (CNNs) are a specialized type of [[Neural Networks|neural network]] designed to process and classify images

# Input Layers

- Takes in an image in 3 dimensions
	- width
	- height
	- depth
		- In an RGB image, each depth is a different color channel

# Convolutional Layers

- Responsible for feature extraction
- Works by appying a set of filters (kernels) that slide over the image computing the dot product between the kernel and the part of the image covered by it
	- Kernels are small matrices of numbers
	- These numbers are decided by the effect desired from the kernel
		- e.g. edge detection, blurring, sharpening
	- The output of this process is known as the feature map

## Stride

- Number of pixels by which a kernel moves across the input image
- Increasing the stride reduces output dimensions

## Padding

- Number of extra pixels added around the edges of the input image
- This is done to preserve the information at the edges of the image

# Pooling Layers

- Responsible for dimensionality reduction
- 2 types
	- Max pooling
		- Take the highest value from the area covered by the kernel
	- Average pooling
		- Take the average of the values from the area covered by the kernel

# Flattening Layers

- Takes in the entire feature map, and reorganizes it into a single long vector
- This is done because classification layers (dense layers) are designed to operate on 1-dimensional data

# Activation Functions

- [[Neural Networks#Activation Functions|As in simple neural networks]] CNNs also have activation functions
	- However, not every layer has them
		- Usually between [[#Convolutional Layers|convolutional layers]] and [[#Pooling Layers|pooling layers]]
- Most common activation function in CNNs is ReLU
	- If input is positive output it directly, else output 0