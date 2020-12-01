# CNNPyTorchAndPyTorchLightningNMIST
This repository contains the CNN for the nMist dataset downloaded from: https://www.kaggle.com/lubaroli/notmnist
It contains the PyTorch Convolutional Neural Network and the PyTorch Lightning Convolutional Neural Network for the notMNIST dataset. Each of these files have a constructor with the activation funs nn.Conv2d, nn.ReLU(), and nn.MaxPool2d. The selected hyperparameters of in_channels, out_channels, kernel_size, and padding were chosen based on the equation:
O = ((W-K+2P)/S)+1, where O is the output height/length, W is the input height/length, K is the filter size, P is the padding, and S is the stride.
The Forward function passes these results to the next activation function and finally returns the result.
For the PyTorch CNN, the training and testing are performed by the def train_test. To run the training dataset, first pass the testing_loader and then the training_loader. To run the testing dataset, first pass the training_loader and then the testing_loader.
For the PyTorch Lightning CNN, the def training_step and def configure_optimizers take care of the training and testing.


