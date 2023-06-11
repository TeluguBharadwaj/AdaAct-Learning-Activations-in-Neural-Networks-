# Learning Activations in Neural Networks

Abstract—The choice of Activation Functions (AF) has proven to be an important factor that affects the performance of an Artificial Neural Network (ANN). Use a 1-hidden layer neural
network model that adapts to the most suitable activation function according to the data-set. The ANN model can learn for itself the best AF to use by exploiting a flexible functional form,
k0 + k1 ∗ x with parameters k0, k1 being learned from multiple runs. You can use this code-base for implementation guidelines and help. https://github.com/sahamath/MultiLayerPerceptron

I. BACKGROUND

Selection of the best performing AF for classification task is essentially a naive (or brute-force) procedure wherein, a popularly used AF is picked and used in the network for
approximating the optimal function. If this function fails, the process is repeated with a different AF, till the network learns to approximate the ideal function. It is interesting to inquire
and inspect whether there exists a possibility of building a framework which uses the inherent clues and insights from data and bring about the most suitable AF. The possibilities
of such an approach could not only save significant time and effort for tuning the model, but will also open up new ways for discovering essential features of not-so-popular AFs.

II. MATHEMATICAL FRAMEWORK

A. Compact Representation
Let the proposed Ada-Act activation function be mathematically defined as
                                     g(x) = k0 + k1x
where the coefficients k0, k1 and k2 are learned during training via back-propagation of error gradients

