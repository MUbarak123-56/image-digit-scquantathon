# Simple Block - Zero Or One Image Digit Classification (South Carolina Quantathon Competition)

## Introduction

This project was conducted as part of the IonQ Quantum Vision Challenge at South Carolina Quantathon which was hosted by the Darla Moore School of Business at the University of South Carolina. The objectivre of this project is to devise a quantum layer within a hybrid quantum-classical neural network that is designed to differentiate between the digits 0 and 1. The quantum layer in this architecture is expected to perform a different role compared to the traditional quantum-classical neural network where the training is done using a lot of the classical layers with just one or two quantum layers involved in the training process. The quantum layer here is expected to conduct most of the training on the data set. Below are figures to display the different sections of the architecture.

![Pre-processing](images/convolution.png)


The image above showcases the pre-processing step of the algorithm. This aspect focuses on flattening the image into 784 vector while using PCA to reduce its size to 168 dimensions before being fed into the quantum layer.

![Quantum Layer](images/quantum_layer.png)

The quantum layer is the section of the algorithm where all the training is going to take place. The scope of this project is to define an effective quantum layer that can yield meaningful reproducible results while training on a small set of data.

![Post-Processing](images/final_layer.png)

Finally, the post-processing step translate the output from the quantum layer into 0 or 1 by working with a fully connected layer to produce a value of 0 or 1 in the last output neuron.

## Problem Statement

With the emergence of Quantum Computing and its potential to tackle complex computations, research on newer domains such as quantum machine learning and quantum optimization are being rigorously conducted with the expectation of developing newer ideas for tackling problems that we have always struggled with. Although quantum machine learning is not as great as its classical counterparts, there is a lot of room for improvement when it comes to innovating within the field. Therefore, the major objective of this project is to develop a quantum circuit that can pave way for future development within the quantum machine learning ecosystem.

## Methodology

The methodology was to develop a quantum layer that can act as a component within the neural network. Our objective was three-fold: simplicity, training speed and reproduciboility. This quantum layer will be simple while being able to yield reproducible results and training data within a reasonable period of time. Therefore, we began by transforming the initial circuit into a simpler circuit by replacing the Angle Encoder with the ZFeatureMap, a simpler data encoding mechanism. We also used a new method for convolution by drawing inspiration from Qiskit's [Tutorial](https://qiskit-community.github.io/qiskit-machine-learning/tutorials/11_quantum_convolutional_neural_networks.html) on Quantum Convolution Neural Network.

![First Attempt](images/qcnn_z_feature_map.png)

After struggling to get a stabilized result with the algorithm above, it was crucial to explore simpler methods. Moreover, the algorithm above took a long period to train (about 200 seconds per epoch). As this is a 24-hour hackathon

## Solution

## Conclusion
