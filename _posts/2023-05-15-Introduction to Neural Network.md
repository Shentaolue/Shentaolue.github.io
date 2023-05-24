## Neural Network - Introduction
Neural Network is a significant technique in AI, it drives the development of Deep Learning techniques. It is the base of those advanced Deep Learning models, such as CNN, RNN, GAN etc. The Neural Network is very flexible, as it has many usage and can be applied to a lot of cases, such as time-series forecasting problem, image classification, Language processing etc. It is powerful and adaptive to different needs.

## Structure of Neural Network
<img src="/images/ANN1.png" width="500" height="230">
<br>
This is a typical structure of Neural Network. The model basically has 3 layers, input layer, hidden layer and output layer. The inputs are passed to the input layer, which is connected to the neurons inside the hidden layer. Each of the neurons will perform the expression shown in the image. The output of the neurons will be the sum of previous input, multiplied by the corresponding weight and added by the bias, and perform the **activation function**. After the inter-connected layer by layer of neurons inside the hidden layer, the complex expression of the data will be expressed by each of the unique weight and bias inside the neurons.
## Activation Function
Activation function is an essential part of Neural Network. Without the activation funcition, the output of Neural Network is just a combination of multiple linear expressions, which won't be able to express the complex pattern from data. However, the use of activation function enables the model to experss non-linear relations. The typical activation functions are ReLU, Tanh, sigmoid etc. The different activation has different effect on the performance of Neural Network. It is good to try different methods and compare the performance for each of them.
<img src="/images/nn1.png" width="270" height="150">
## Loss Function
Loss Fucntion is used to measure the difference between the output of the model and the expected result, to reflect how good the model is performing. Accoding to the course, MSE(Mean Squared Error) is the loss funcition that is commonly used. <br> 
<img src="/images/nn2.png" width="320" height="35">
<br>
With the loss measured by the loss function, we can do the backpropagation by finding the gradient of the loss, to update the weights and biases inside the layers. This will be done by using the optimizer funciton (Adam Optimizer as an example). There are many choices of loss funcitons, such as MSE, BCD, CrossEntrophy. The choose of loss function should consider the usage of the model. CrossEntrophy loss function is quite common in image classification. The following table shows the choices of loss funciton according to the usage.
<br> 
<img src="/images/nn3.png" width="300" height="400">
<br>
## Optimizing function 
After calculating the loss and gradient, the optimizing function will be used to update the parameters inside the layers, in order to reduce the error. The rate of modifying the parameters depends on the learning rate specified. The common optimizer functions are:
- Adam Optimizer
- Stochastic Gradient Descent (SGD)
- AdaGrad
The choice of Optimizing function depends on the training dataset and the use of the model. Different optimizer will have large difference on the model performance.

## Conclusion
The Neural Network is an extremely important model in the development of AI. It is capable of capturing the non-linear relation from the data. The choice of Loss function, optimizing funciton is very crucial for the model.
