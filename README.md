# Guided-Deep-Dreaming
An implementation of Guided Deep Dreaming using Caffe

# Introduction
DeepDream is a computer vision program created by Google which uses a Convolutional Neural Network to find and enhance patterns in images via algorithmic pareidolia, thus creating a dreamlike hallucinogenic appearance in the deliberately over-processed images.

This repo demonstrates 'Guided' Deep Dreaming. It is possible to guide the dreaming process by supplying a seed image. The seed image is used to guide and influence the output.

# Source
http://www.pyimagesearch.com/2015/07/13/generating-art-with-guided-deep-dreaming/

Thank you for the amazing tutorial Mr. Adrian Rosebrock!

# Requirements
Requires Caffe (http://caffe.berkeleyvision.org/) to be installed with Python 2.7.

Also requires bat-country package to be installed. To do so, type:


`pip install bat-country`


# Usage (on Ubuntu)
Open the terminal. cd to the directory containing the deepdream.py file.

Now, run the program by passing arguments to it:

python deepdream.py [-h] -b BASE_MODEL [-l LAYER] -i IMAGE -g GUIDE_IMAGE -o OUTPUT

[ ] means that the argument is optional.

-h means help

-b BASE_MODEL is the base model path (path to CNN model (.cafemodel file) on your machine)

-l LAYER is the layer of the CNN to be used. If GoogLeNet is used, inception_4c/output is the default. Try conv2/3x3 and inception_3b/5x5_reduce also!

-i IMAGE is the path to the input image that is to be modified

-g GUIDE_IMAGE is the path to the guide image that will be used while dreaming

-o OUTPUT is the path to the output image
