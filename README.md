# Handwritten Number Detector ✍️✍️
Description 📃📃:
This project delves into the world of digit recognition using the MNIST dataset, a classic in computer vision. The goal was to develop models capable of accurately identifying handwritten digits. My initial thought was to use a logistic regression but having 70,000 examples felt like it would be a waste and then tried a deep neural network with 100 hidden layers which provided better predictions.
 
## Dataset 🗃️🗃️
The data set is the Modified National Institute of Standards and Technology database (MNIST). The MNIST dataset is a large collection of handwritten digits. Imported from sklearn.datasets library. It consists of 70,000 training examples of square 28×28 pixel images of handwritten single digits between 0 and 9 and 10,000 testing examples.

mnist = sklearn.datasets.fetch_openml('mnist_784')

## Geeky specs 🤓🤓
The model uses the Adam optimizer because it combines elements of two other popular optimizers: RMSprop and AdaGrad, to provide an efficient and effective optimization technique. 
Since this model has multi-class classification problems where the labels are integers as the prediction outputs sparse categorical cross-entropy was used as the loss function.
There is a hidden layer with 100 neurons in the model with the Relu(Rectified Linear Unit) activation function and the input and output layers fit with the sigmoid activation function.

## Models 🔩🔩
The accuracies on the testing set of the models I used are the following
Logistic Regression: 92.58%

Neural Network: 92.54%

Deep Neural Network: 97.46% 
