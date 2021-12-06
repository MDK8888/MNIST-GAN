# MNIST-GAN

## Project Overview:
This Repository contains my implementations of a Generative Adversarial Network(GAN) trained on the MNIST Image Recognition Dataset. GANs are one type of generative Deep Learning Model. The GAN consists of 2 different Neural Networks, a Generator which generates fake images from random numbers and a Discriminator which attempts to tell fake and real images from the dataset apart. In training, the Generator attempts to "fool" the Discriminator into classifying its fake images as real ones, and the Discriminator attempts to discern which images are real and which ones are fake. All three implementations were built and trained entirely in Numpy without the aid of Tensorflow/Keras or Pytorch. The file titled "MNIST GAN Perfect" is the final version of the model and the resolution of the generated images is much clearer on this version than on previous versions. 

## Final Model Implementation Details:
**Loss Function:** Jensen-Shannon Divergence

**Optimizer:** ADAM with the learning rate = 0.0002, β1 = 0.5, β2 = 0.999

**Training Epochs:** 10

**Batch Size:** 50

**Additional Techniques:** Instance Noise 

**Generator Architecture:** Fully Connected Neural Network w/ Batch Normalization after ReLU Activation

Latent Space dim: 100

1st Hidden Layer dim: 128

2nd Hidden Layer dim: 256

3rd Hidden Layer dim: 512

4th Hidden Layer dim: 1024

**Discriminator Architecture:** Fully Connected Neural Network w/ ReLU Activation

Input dim: 784

1st Hidden Layer dim: 628

2nd Hidden Layer dim: 471

3rd Hidden Layer dim: 314

4th Hidden Layer dim: 157
