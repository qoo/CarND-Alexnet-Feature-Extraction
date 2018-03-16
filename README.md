# AlexNet Feature Extraction
[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)

This lab guides you through using AlexNet and TensorFlow to build a feature extraction network.

## Setup
Before you start the lab, you should first install:
* Python 3
* TensorFlow
* NumPy
* SciPy
* matplotlib

## Instruction
```
Transfer Learning with TensorFlow
Transfer learning is the practice of starting with a network that has already been trained, and then applying that network to your own problem.

Because neural networks can often take days or even weeks to train, transfer learning (i.e. starting with a network that somebody else has already trained) can greatly shorten training time.

How do we apply transfer learning? Two popular methods are feature extraction and finetuning.

Feature extraction. Take a pretrained neural network and replace the final (classification) layer with a new classification layer, or perhaps even a small feedforward network that ends with a new classification layer. During training the weights in all the pre-trained layers are frozen, so only the weights for the new layer(s) are trained. In other words, the gradient doesn't flow backwards past the first new layer.

Finetuning. This is similar to feature extraction except the pre-trained weights aren't frozen. The network is trained end-to-end.

The labs in this lesson will focus on feature extraction since it's less computationally intensive.

Getting Started
Set up your environment with the Udacity CarND Starter Kit.
Clone the repository containing the code.
git clone https://github.com/udacity/CarND-Alexnet-Feature-Extraction
cd CarND-Alexnet-Feature-Extraction
Download the training data and AlexNet weights. These links are also available at the bottom of this page under Supporting Materials.
Make sure the downloaded files are in the same directory as the code.
Open the code in your favorite editor.
Feature Extraction via AlexNet
Here, you're going to practice feature extraction with AlexNet.

AlexNet is a popular base network for transfer learning because its structure is relatively straightforward, it's not too big, and it performs well empirically.

There is a TensorFlow implementation of AlexNet (adapted from Michael Guerhoy and Davi Frossard) in alexnet.py. You're not going to edit anything in this file but it's a good idea to skim through it to see how AlexNet is defined in TensorFlow.


The team behind AlexNet. Source: Wired.

Coming up, you'll practice using AlexNet for inference on the image set it was trained on.

After that, you'll extract AlexNet's features and use them to classify images from the German Traffic Sign Recognition Benchmark dataset.

Credits
This lab utilizes:

An implementation of AlexNet created by Michael Guerzhoy and Davi Frossard
AlexNet weights provided by the Berkeley Vision and Learning Center
Training data from the German Traffic Sign Recognition Benchmark
AlexNet was originally trained on the ImageNet database.

Supporting Materials
 Train
 Bvlc Alexnet Weights
```
