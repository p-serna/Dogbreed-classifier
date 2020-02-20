# Dog breed classifier

Dog breed classifier project for Udacity

## About

This is a repository for a dog breed classifier. It contains sources to an application that determine if a picture contains a dog, a human or something else, and in the case of a dog or human, to which dog breed the individual would belong.  Following/forked [udacity repository](https://github.com/udacity/deep-learning-v2-pytorch).

The app is presented as two-steps solution. First, we used standard algorithms to determine if the picture indeed has a dog or a human. To detect a human in pictures we used a face detector implemented in OpenCV, based on Haar cascades. Then for detecting whether there is a dog or not, we use the state-of-the-art mobilenet v2 model. Finally, if any of the previous algorithms gives a positive answer, we provide the image to a custom network that classifies it into 133 possible breeds. The custom network is either a convolutional network trained from scratch or a networkwith the architecture of mobilenet v2, where we used transfer-learning techniques, adapted to 133classes.

<img src="scheme.png" alt="Scheme of two-steps solution" style="width: 100%;"/>

## For Review

- Data exploration notebook: [pdf](data exploration.pdf) or [html](data exploration.html).
- Dog app notebook: [pdf](dog_app.pdf) or [html](dog_app.html).
  
  

## Datasets

Dogs Database - Udacity

Labeled Faces in the Wild (LFW) [database](http://vis-www.cs.umass.edu/lfw/).

> [Gary B. Huang](http://vis-www.cs.umass.edu/%7Egbhuang), Manu Ramesh, [Tamara Berg](http://research.yahoo.com/bouncer_user/83), and [Erik Learned-Miller](http://www.cs.umass.edu/%7Eelm). **Labeled Faces in the Wild: A Database for Studying Face Recognition in Unconstrained Environments.**  
> *University of Massachusetts, Amherst, Technical Report 07-49*, October, 2007. [Gary B. Huang](http://vis-www.cs.umass.edu/%7Egbhuang) and [Erik Learned-Miller](http://www.cs.umass.edu/%7Eelm). **Labeled Faces in the Wild: Updates and New Reporting Procedures.**  
> *University of Massachusetts, Amherst, Technical Report UM-CS-2014-003*, May, 2014.

## Getting Started

Follow the jupyter notebook of data exploration to get to know the datasets. Then use the dog_app notebook to set up the training and developed algorithms._

## Requirements

- Pytorch

- Pytorch vision

- Numpy

- Matplotlib
