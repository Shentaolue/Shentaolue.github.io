## What is fastai?
AI technology is complicated. Building an AI model from scartch is complex, time consuming and extremely difficult -- almost impossible for a student like me. However, the fastai is created to save us! fastai is a framework that helps the researchers build their model from a top design level, which means, researchers only need to learn how to use the model, without learning how does the low-level computations work. This saves a lot of precious time and energy to a beginner in AI area.<br><br>
## PyTorch Library
The fastai library is built upon PyTorch framework. From the course we know that PyTorch has become a dominating framework that the researchers prefer to use since recent years. It will greatly help researchers following the latest AI techniques including papers, models based on PyTorch instead of other frameworks.

<img src="/images/pytorchvstensorflow.png" width="400" height="240">

The PyTorch Library is awesome. Let's look at an example from PyTorch tutorial:
[link to tut](https://pytorch.org/tutorials/beginner/blitz/cifar10_tutorial.html).
<br><br>
To build a CNN model doing image classification, we start from processing the dataset. In python we usually use Dataloader to do processing on training set, validation set and testing set separately. After preparing the dataset, we can actually building the model. User needs to custmize the model by specifying the layers, sizes, and defining the transitions between each layer.<br>
<img src="/images/pytorch_example.png" width="380" height="300">
<br>
Then, we need to design the loss function and optimizer function. After this, we need to use for loop to do the training and testing. We need to create array to record the losses, and use print to see the loss details.<br>
<img src="/images/pytorch_example2.png" width="380" height="290">
<br>
Finally, we can do testing on the model. Honestly speaking, althogh the PyTorch procedure is good for understanding the models, and provide the freedom for users customize the models, the procedure of PyTorch is quite complicated, which might not be very friendly to the beginners. And for the experienced researchers, they might spend many time on setting up the model, doing data preparing, and debugging during the process. This is very time consuming. However, let's see how to build a classifier in fastai.<br>
## fastiai classifier
If we build a classifier in fastai, as Jeremy showed in his video, the dataset is prepared by using "dataloader", and the model training is shown as follows:<br>
<img src="/images/fastai1.png" width="320" height="180">
<br>
In this 2 lines of code, a CNN model is designed and already starts to training!<br>
And the very cool thing is, the training process is shown in the progress bar, the user can easily see how the training going, with the training loss and validation loss avaliable.<br><br>
After training the model, testing the model is also very simple. Simply use "learn.predict" function to do the classification, the result will be obtained.<br>
<br>
<img src="/images/fastai2.png" width="320" height="80">
<br>
## Conclustion
The fastai library provides researcher a fast and easy way to use the AI models, aiding researchers focusing on the designing instead of the implementation work. However, this is just a small part of fastai, there are far more functionality which are flexible, easy to use and powerful in fastai waiting to be discovered. It is definately worth exploring and practicing different functionality in fastai!

