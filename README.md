# Deep Learning & Art: Neural Style Transfer
This is one of the Week 4 programming assignments on Convoluted Neural Network in [deeplearing.ai](https://www.coursera.org/specializations/deep-learning)

## Summary
Generating novel artistic images with Neural Style Transfer (NTS). Neural Style Transfer is an algorithm, that given a content image C and a style image S, can generate an artistic image.

It uses representations (hidden layer activations) based on a pre-trained ConvNet. The content cost function is computed using one hidden layer's activations; the style cost function for one layer is computed using the Gram matrix of that layer's activations. The overall style cost function is obtained using several hidden layers.

Lastly, optimizing the total cost function results in synthesizing new images.

## Citations & References
The Neural Style Transfer algorithm was due to Gatys et al. (2015). Harish Narayanan and Github user "log0" also have highly readable write-ups from which we drew inspiration. The pre-trained network used in this implementation is a VGG network, which is due to Simonyan and Zisserman (2015). Pre-trained weights were from the work of the MathConvNet team.

* Leon A. Gatys, Alexander S. Ecker, Matthias Bethge, (2015). [A Neural Algorithm of Artistic Style](https://arxiv.org/abs/1508.06576)

* Harish Narayanan, [Convolutional neural networks for artistic style transfer](https://harishnarayanan.org/writing/artistic-style-transfer/).

* Log0, [TensorFlow Implementation of "A Neural Algorithm of Artistic Style"](http://www.chioka.in/tensorflow-implementation-neural-algorithm-of-artistic-style).

* Karen Simonyan and Andrew Zisserman (2015). [Very deep convolutional networks for large-scale image recognition](https://arxiv.org/pdf/1409.1556.pdf)

* [MatConvNet](https://www.vlfeat.org/matconvnet/pretrained/).
