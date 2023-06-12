# Learning Activations in Neural Networks

Introduction:

Artificial Neural Networks (ANNs) have emerged as powerful models for solving complex classification tasks. The success of ANNs heavily relies on the choice of activation functions, which introduce non-linearity and enable the network to learn complex representations. The selection of an appropriate activation function plays a critical role in achieving accurate predictions and improving the overall performance of neural networks.Traditionally, fixed activation functions such as sigmoid, tanh, and ReLU have been widely used in neural network architectures. However, these fixed activation functions have inherent limitations. They are designed based on certain assumptions and may not be universally optimal for all datasets. This raises the question of whether it is possible to build a framework that can adaptively learn and select the most suitable activation function based on the characteristics of the dataset

This project aims to develop a 1-hidden layer neural network model that adapts to the most suitable activation function based on the dataset. The model employs a flexible functional form, k0 + k1 * x, where the parameters k0 and k1 are learned through multiple training runs. The training process involves updating the model's parameters, including weights, biases, and activation function coefficients, over multiple epochs using the Adam optimizer. The performance of the model is evaluated based on train and test loss, train and test accuracy, and the F1-Score. The experimental results demonstrate the effectiveness of the adaptive activation function approach in achieving accurate classification. The report provides insights into the algorithm, initial parameter settings, parameter updates on epochs, final parameter values, and presents a plot of the loss function vs. epochs, highlighting the model's learning progress.

Implimentation summary:

The implementation incorporates a 1-hidden layer neural network model that adapts to the most suitable activation function according to the dataset. The activation function used in the hidden layer is represented by the equation g(x) = k0 + k1 * x, where k0 and k1 are learned during training.

The implementation utilizes the Iris dataset for experimentation, which is preprocessed by performing one-hot encoding on the target variable and scaling the input features. The dataset is then split into training and testing sets.

The model architecture consists of a sequential model with one hidden layer of 25 units. The custom activation function, Adaact, is implemented using the equation g(x) = k0 + k1 * x. Dropout regularization is applied after the hidden layer to prevent overfitting. The output layer uses the softmax activation function for multi-class classification.

The model is trained using the Adam optimizer and categorical cross-entropy loss function. The training process is conducted for a specified number of epochs, and the performance metrics, including train and test loss, train and test accuracy, and F1-score, are evaluated. The loss function is plotted against the epochs to visualize the model's learning progress.

The experiment results demonstrate the effectiveness of the model in adapting the activation function. The train and test loss values, along with the train and test accuracy, provide insights into the model's performance. The F1-score further evaluates the model's classification performance

In conclusion, the approach of adapting the activation function based on the dataset shows promise in improving the performance of neural networks. The inclusion of the equation g(x) = k0 + k1 * x allows the model to learn the optimal activation function parameters, leading to enhanced approximation of the target function. Further research and exploration can be conducted to investigate the potential of this approach in other domains and datasets.

Datasets used: Iris,MNSIT,Wisconsin Breast Cancer,Bank Note

