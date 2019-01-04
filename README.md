# Fast-and-efficient-binarized-variational-autoencoders
Deep neural networks perform extremely well in several application domains including computer vision,
speech recognition etc. In computer vision applications Variational Autoencoders, have demonstrated
state-of-the-art results in being able to capture a good representation of the data. However, these
convolution based recognition systems occupy a large amounts of memory and are quite expensive in
terms of computational power. While they perform well on expensive, GPU-based machines, they are
quite unsuitable for smaller devices like cell phones and embedded electronics.
Here, we propose to model a simple, efficient and accurate approximation of a Variational Autoencoder
by binarizing their weights and even their intermediate layers to learn an approximately representation
of the input sample. The method aims at finding the best approximation of the convolution using
binary operations. Since binarizing the parameters of the network leads to challenges during learning
i.e. during backpropogation (non-differentiable), We aim to learn this binary approximation function,
keeping almost the same reconstruction as when the weight are real valued numbers.
One variation which we would like to attempt is to study the reconstructed output of an unseen class
using inference time, which basically attempts to understand whether this new network is able to learn
the spatial representation of an image using binary parameters
