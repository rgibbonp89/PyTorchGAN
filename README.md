# PyTorchGAN

In this repo you'll find my coding of a simple generative adversarial network. I realized a little while ago that I wanted a better understanding of how GANs work, so I decided to write one in PyTorch as well as a brief presentation on how they work. My suggestion would be to read my presentation alongside the code, then run it all and look at the results. Also, you'll need to download the data if you haven't already. Grab it from [here](http://yann.lecun.com/exdb/mnist/) and save it in the same directory as the .py file in a ./data subdirectory. 

My plan is to, at some point, do a similar thing for a couple of other GAN variants (DCGAN, CGAN, WGAN, etc.), but that'll have to wait for a little bit. 

To run the code, just call the following in your terminal:

python3 torchGAN.py --number [number that you want to generate] --epochs [the number of epochs] --glr [the generation learning rate] --dlr [the discriminator learning rate]
  
If you don't specify anything for the command line arguments, the code just executes with default settings.

## Fashion-MNIST

I've also added support for fashion-MNIST, so you can generate images from that dataset, too. The default command line arguments are the same, but you can also specify --mnist as either 'digits' or 'fashion'.

You'll also need to save the fashion-MNIST data locally. I'd recommend the following:

1. Install tensorflow
2. Run from tensorflow.examples.tutorials.mnist import input_data in python
3. Run data = input_data.read_data_sets('data/fashion', source_url='http://fashion-mnist.s3-website.eu-central-1.amazonaws.com/', one_hot=True)
4. Unpack the downloaded .gz file and put it in a ./fashion subdirectory in the same directory as the original MNIST data

Enjoy!
