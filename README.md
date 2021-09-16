# Miniature Popular CovNets

![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white) ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) ![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)

In mathematics, a convolution casually speaking, is a mixture of two functions. In machine learning, a convolution mixes the convolutional filter and the input matrix in order to train weights.

Without convolutions, a machine learning algorithm would have to learn a separate weight for every cell in a large tensor. When the convolutional filter is applied, it is simply replicated across cells such that each is multiplied by the filter.

**Source :** [Google Developers Machine Learning ](https://developers.google.com/machine-learning/glossary#convolution "Google Developers Machine Learning ")

This notebook has **miniature versions** of a few most popular convolutional neural networks.

### About CovNets

------------

- **VGG Network**
	The runner-up in the ILSVRC 2014 challenge was VGGNet. It had a very simple and classical architecture, with 2 or 3convolutional layers and a pooling layer, then again 2 or 3 convolutional layers and apooling layer, and so on (reaching a total of just 16 or 19 convolutional layers, depending on the VGG variant), plus a final dense network with 2 hidden layers and the output layer. It used only 3 × 3 filters, but many filters.

- **Inception Network**
	GoogLeNet won the ILSVRC 2014 challenge by pushing the top-five error rate below 7%, it actually has 10 times fewer parameters than AlexNet which is possible because of subnetworks called **inception modules**, that allow GoogLeNet to use parameters much more efficiently than previous architectures.

	![Inception Module](https://i.ibb.co/x3RWHJF/Screenshot-63.png "Inception Module")

- **ResNet or Residual Network**
	ResNet won the ILSVRC 2015 challenge using a **Residual Network** that delivered an astounding top-five error rate under 3.6%. The winning variant used an extremely deep CNN composed of 152 layers, The key to being able to train such a deep network is to use **skip connections**. the network is forced to model `f(x) = h(x) – x` rather than `h(x)`. This is called residual learning.

	![Skip Connection](https://i.ibb.co/8xfKddh/Screenshot-64.png "Skip Connection")


Reference : [Hands-On Machine Learning with Scikit-Learn and TensorFlow](https://www.oreilly.com/library/view/hands-on-machine-learning/9781491962282/ "Hands-On Machine Learning with Scikit-Learn and TensorFlow") 
