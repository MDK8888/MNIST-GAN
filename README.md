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
## GAN Real Images
![MNIST Real Image Sample2](https://user-images.githubusercontent.com/79173446/150605415-519715fd-03c8-48b4-9be5-33d86a3ff6fc.PNG)
![MNIST Real Image Sample1](https://user-images.githubusercontent.com/79173446/150605445-ea27f4f0-12eb-4ad0-aebb-952d922d83ce.PNG)
![MNIST Real Image Sample3](https://user-images.githubusercontent.com/79173446/150605455-82fa2369-3d71-4ed7-b6f2-ed0a677929d7.PNG)
## GAN Generated Image
![MNIST Generated Image Sample](https://user-images.githubusercontent.com/79173446/150605506-bc76327a-17e7-4731-a6f0-61a7760849bb.PNG)

