# Extreme-Sparsity-by-Input-Monotone-Neural-Networks

# Brief Description

Every function R^D-> R can be represented as a sum of monotone decreasing and increasing functions. Thus, one may consider learning any function by a pair of monotone increasing and decreasing Neural Networks. Monitonicity can be achieved via using monotone activations and keeping some weights of the network positive. The potential advantage of this approach is SPARSITY which naturally arises due to weight clamping (although this may reduce expressiveness & complicate training). This project is to study this expressiveness & sparsification ability of such networks.	

# General Project Goals
Consider classical Fully Connected & Convolutional architectures (such as ResNet, U-Net, AlexNet), "monotonize" them. Test the performance of such networks on various datasets to assess whether they can provide nearly state-of-the-art performance. Report the sparsification of the networks. 
Consider same setup with additional L1-regularization (or Group-LASSO).	"

# Tasks
- For each of the networks fetch a dataset (MNIST for FC network, Cats/Dogs for Alex-Net, Cifar-100 for ResNet, some segmentation problem for U-Net, some Convolutional AE for CelebA dataset)
- Train networks (1-net-per-task): try to achieve nearly state-of-the-art performance (you can use any code from github to do this, NO NEED to write it on your own)
- In the same scenario, train the ""monotone"" versions of such networks. Collect the resulting scores (& convergence) and report the sparsity.
- Same monotone scenario, but with L1-regularization on the weights
- In all the considered cases of monotone networks, performs sanity checks to confirm that your networks are indeed input-monotone"	
- 
# Ref
https://arxiv.org/abs/1512.03385
https://arxiv.org/abs/1505.04597
https://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks.pdf"
