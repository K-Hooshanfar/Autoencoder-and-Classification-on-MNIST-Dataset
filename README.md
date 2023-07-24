# Autoencoder-and-Classification-on-MNIST-Dataset


This code consists of two main parts. The first part is an autoencoder designed to compress and decompress MNIST handwritten digit images, and the second part is a classification model that uses the output of the encoder as input.


## Requirements
keras -
numpy -
matplotlib -
tensorflow -
pandas -
seaborn -
sklearn


## Data Preprocessing
The code loads the MNIST dataset and preprocesses the data by normalizing the pixel values to be in the range [0, 1].

## Autoencoder
The autoencoder is designed with three hidden layers. The latent space size is set to 30. The model is trained on the MNIST dataset for 100 epochs using the Adam optimizer and binary cross-entropy loss. The autoencoder is then evaluated by comparing the original and reconstructed images, and plotting the loss and validation loss over the training epochs.



## Classification
The output of the encoder is used as the input for the classification model. The classification model has two hidden layers, each with 30 neurons, and an output layer with 10 neurons representing the 10 classes in the MNIST dataset. The model is trained for 10 epochs using the Adam optimizer and categorical cross-entropy loss. The classification model is evaluated by calculating the accuracy and confusion matrix on the test data.

## Results
The autoencoder is able to effectively compress and reconstruct the MNIST images, with a validation loss of around 0.08 after 100 epochs of training. The classification model achieves an accuracy of over 97% on the test data.
![96bd57d0-f0c6-44c1-bb55-3d10a8aac407](https://github.com/K-Hooshanfar/Autoencoder-and-Classification-on-MNIST-Dataset/assets/83825004/3c5a9c45-193e-4e88-a5d1-47564877f63e)

*Train/Val accuracy and loss plot*

![d660f7bd-2d4d-44fe-89fb-62d0eef31ae6](https://github.com/K-Hooshanfar/Autoencoder-and-Classification-on-MNIST-Dataset/assets/83825004/e71882e1-aa98-436f-b881-c653987e80ae)

*Confusion Matrix*




