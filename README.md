# cifar10

An image classification model using Convolution Neural Network.

The model is trained on the Cifar10 dataset, which has a total of 60,000 images divided into 10 classes.
The dataset is as follows.

![Cifar10 Dataset](https://appliedmachinelearning.files.wordpress.com/2018/03/cifar2.jpg?w=427)

We use the process of DataAugmentation to create more training data for better results.

The model uses the following architecture :-

(Conv2D -> Relu -> BatchNorm)*2 -> (maxpool -> Dropout -> (Conv2D -> Relu -> BatchNorm)*2 )*2 -> Maxpool -> Dropout ->
Flatten -> (Dense -> Relu -> Dropout)*2 ->  Dense -> Softmax.

The model attains an accuracy of nearly 80% in 50 epochs.
The model can be trained for a longer time for better results.
