# Simple Block - Zero Or One Image Digit Classification (South Carolina Quantathon Competition)

## Introduction

This project was conducted as part of the IonQ Quantum Vision Challenge at South Carolina Quantathon which was hosted by the Darla Moore School of Business at the University of South Carolina. The objectivre of this project is to devise a quantum layer within a hybrid quantum-classical neural network that is designed to differentiate between the digits 0 and 1. The quantum layer in this architecture is expected to perform a different role compared to the traditional quantum-classical neural network where the training is done using a lot of the classical layers with just one or two quantum layers involved in the training process. The quantum layer here is expected to conduct most of the training on the data set. Below are figures to display the different sections of the architecture.

![Pre-processing](images/convolution.png)
*Figure 1: Pre-processing step*


The image above showcases the pre-processing step of the algorithm. This aspect focuses on flattening the image into 784 vector while using PCA to reduce its size to 168 dimensions before being fed into the quantum layer.

![Quantum Layer](images/quantum_layer.png)
*Figure 2: Quantum Layer*

The quantum layer is the section of the algorithm where all the training is going to take place. The scope of this project is to define an effective quantum layer that can yield meaningful reproducible results while training on a small set of data.

![Post-Processing](images/final_layer.png)
*Figure 3: Post-Processing Step*

Finally, the post-processing step translate the output from the quantum layer into 0 or 1 by working with a fully connected layer to produce a value of 0 or 1 in the last output neuron.

## Problem Statement

With the emergence of Quantum Computing and its potential to tackle complex computations, research on newer domains such as quantum machine learning and quantum optimization are being done rigorously with the expectation of developing different mechanisms for tackling problems that we have always struggled with. The main problem of this experiment is to see if a quantum algorithm that can 

## Solution

## Conclusion
