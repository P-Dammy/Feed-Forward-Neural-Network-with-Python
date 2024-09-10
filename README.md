**1. Introduction**

The Iris dataset is a well-known dataset in the field of machine learning, commonly used for classification tasks. This project implements a Feedforward Neural Network (FNN) using Keras and TensorFlow to classify the Iris flowers into one of three species: Setosa, Versicolor, or Virginica. The network is trained using various techniques and evaluated on how well it performs in classifying the species based on four input features.

The goal of this project is to demonstrate the effectiveness of FNN in handling small, structured datasets like Iris and to gain insights into the behavior of the network in a multi-class classification problem.

**#2. Data Description**
The Iris dataset consists of 150 samples, with the following features:

**sepal length (cm)
sepal width (cm)
petal length (cm)
petal width (cm)**
The target variable (species) consists of three classes:

**Setosa
Versicolor
Virginica**
Each class contains 50 samples. The dataset is balanced, making it ideal for demonstrating the classification capabilities of a Feedforward Neural Network.

Dataset Source: The dataset can be directly loaded from the sklearn library, or via the seaborn library.

**3. Project Overview**
This project is structured as follows:

**3.1 Data Preprocessing and EDA**
The Iris dataset is first preprocessed by normalizing the input features. This ensures that the neural network can efficiently learn during training. No missing values or categorical features need handling, making the preprocessing minimal. Also, the data wa explored visually for better understanding of the data

**3.2 Model Architecture**
The model is a Feedforward Neural Network (FNN) with:

Two hidden layers, each consisting of 10 neurons and using the ReLU activation function.
The output layer has 3 neurons (one for each class), using the Softmax activation function to output class probabilities.
The model is compiled using:

Loss function: sparse_categorical_crossentropy, as it's a multi-class classification problem.
Optimizer: Adam optimizer, a widely-used optimization technique for neural networks.
Metrics: Accuracy is used to monitor the model performance.

**3.3 Model Training and Evaluation**
The model is trained on 80% of the dataset, with 20% reserved as a validation set. The network is trained over 50 epochs with a batch size of 5. Accuracy and loss metrics are plotted for both the training and validation sets.

**3.4 Visualization**
The performance of the model is visualized using:

Accuracy and Loss Curves: To show the progression of training and validation accuracy/loss over epochs.
Confusion Matrix: To evaluate the classification performance and visualize the correctly and incorrectly classified samples.

#3.5 Results and Insights
The model achieves a high accuracy on both the training and validation sets, demonstrating the effectiveness of the Feedforward Neural Network in classifying Iris species. Insights about model performance, overfitting, and generalization are discussed based on the training curves and confusion matrix.
