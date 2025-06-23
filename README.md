**Rakshith Bodakuntla**

# GAN_using_PyTorch


I used TensorFlow to implement a simple GAN for generating handwritten digits using the MNIST dataset, which contains thousands of 28x28 grayscale images of digits 0 through 9.

Generator: This model takes random noise as input and transforms it through dense and upsampling layers to produce a 28x28 pixel image that looks like a digit.

Discriminator: This is a binary classifier. It takes an image and outputs a probability of whether it’s real (from MNIST) or fake (from the generator).

I set up a training loop where:

For each batch, the discriminator is trained to classify real and fake images correctly.

Then, the generator is updated to fool the discriminator—by making its outputs more convincing.

Sample Outputs:
I generated sample images at Epoch 0, 50, and 100. Initially, the digits looked like noise. By epoch 50, some digit shapes appeared, and by 100, the generator was producing fairly realistic digits.

Loss Plots:
I also plotted the loss curves for both networks. You can see that as training progresses, the discriminator and generator keep adjusting to each other—illustrating the adversarial training dynamic.
