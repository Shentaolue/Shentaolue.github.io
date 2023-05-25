## Introduction to CNN
Convolutional Neural Networks (CNN) is a type of Deep Learning model. It is commonly used in Image processing, as it has the ability to capture the feature in spatial dimension form the dataset. So those multi-dimensional data such as images can be processed by CNN. It is considered as a state-of-art model and is widely used in Image processing and computer vision.

## Structure of CNN
<img src="/images/CNN1.jpg" width="500" height="250"><br>
The structure of CNN model is shown in the above image. As is shown, the input image is processed by the convolutional filters, which will use convolutional filters to do convolution with input and generate the feature map. The purpose of the convolutional filter is to capture the features such as edges, corners or other image patterns from data. The feature map will then
be passed into the max-pooling layer. The functionality of convolutional and max-pooling layer is shown in next section.
<br>
## Convolutional layer
<img src="/images/CNN3.png" width="400" height="200"><br>
CNN uses a convolutional filter (or named kernel) to operate convolution with the input as a sliding window. This helps the model extracting features and patterns contained in the image. The size of kernel is important to the model, as larger size kernel will extract information globally, small size kernel will extract detailed information from the image.


## Max-pooling layer
<img src="/images/CNN2.png" width="400" height="180">
<br>
Basically, the max-pooling layer reduces the dimention of the feature maps, it approximatly replace the feature map from a large size to a smaller size by finding the maximum value in a range. This will increase the efficiency and also has "blur" effect to detect similar pattern more generally.<br><br>
After Max-pooling, there might be further convolutional layer and max-pooling layer connected to further detect the features. Essentially, the final feature map will be flattened by the flatten layer to be a one-dimention array. This array will then be sent to a fully-connected Neural Network to generate an output. This model is just a traditional Neural Network.

## Conclusion
The CNN model is popularly used in image processing and other applications, it can learn the patterns from multi-dimension data such as images.
