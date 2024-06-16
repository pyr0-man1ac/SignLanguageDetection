Indian sign language is a predominant sign language. Since the only disability DHH people have is 
communication and they cannot use spoken languages hence the only way for them to 
communicate is through sign language. Communication is the process of exchange of thoughts and
messages in various ways such as speech, signals, behavior and visuals. Deaf and hard of 
hearing (DHH) people make use of their hands to express different gestures to express their ideas
with other people. Gestures are the nonverbally exchanged messages and these gestures are 
understood with vision. This nonverbal communication of DHH people is called sign language.
Sign language is a visual language and consists of 3 major components:
In this project focus was on producing a model which will recognize “Word level sign 
vocabulary” based hand gestures. 
 
 
 Convolution Neural Network:
A Convolutional Neural Network (CNN) is a type of deep learning algorithm that excels in 
image recognition and processing. It consists of several key components: convolutional layers, 
which apply filters to detect features in the input data and pooling layers, which reduce the 
spatial dimensions through methods like max pooling. The fully connected layers then integrate 
these features to make final predictions. Flattening is used to convert matrix data into a vector for 
input into fully connected layers. Additionally, dropout is a regularization technique employed to 
prevent overfitting by randomly dropping neurons during training. CNNs are widely used in tasks 
such as image classification and object detection, making them a cornerstone of modern 
computer vision applications. Unlike regular Neural Networks, in the layers of CNN, the
neuronsare arranged in 3 dimensions: width, height, depth. The neurons in a layer will only be 
connected to a small region of the layer (window size) before it, instead of all the neurons in a
fully-connected manner. Moreover, the final output layer would have dimensions (number of 
classes), because by the end of the CNN architecture we will reduce the full image into a single
vector of class scores.
• Convolution Layer: In convolution layer we take a small window size that extends to the depth of 
the input matrix. The layer consists of learnable filters of window size. During every iteration we
slid the window by stride size, and compute the dot product of filter entries and input values at a
given position. As we continue this process well create a 2-Dimensional activation matrix that
gives the response of that matrix at every spatial position. That is, the network will learn filters
that activate when they see some type of visual feature such asan edge of some orientation or a
blotch of some color.
• Pooling Layer: We use pooling layer to decrease the size of activation matrix and ultimately 
reduce the learnable parameters. There are two types of pooling:
➢ Max Pooling: In max pooling we take a window, and only take the maximum of 4 values. Lid the
window and continue this process, until an activation matrix half of its original size is formed.
➢ Average Pooling: In average pooling we take average of all values in a window.
• Fully Connected Layer: In convolution layer neurons are connected only to a local region, while 
in a fully connected region, well connect the all the inputs to neurons.
• Final Output Layer: After getting values from fully connected layer, connect them to final layer
of neurons having count equal to total number of classes, that will predict the probability of each 
image to be in different classes.

Results: 

![Screenshot_16-6-2024_235529_](https://github.com/pyr0-man1ac/SignLanguageDetection/assets/120567662/41a4ddbd-d36b-4f6c-aac8-7c7847fb6788)


As shown in the output window the project can classify both the left and right hand. As soon as the hands are visible white landmarks in a black colour frame covers them. And based on input keypoints it classifies the hand gestures accurately that are visible on the screen. It also shows FPS(Frames per second) rate and also can tell the gestures are moving in which direction or are not moving at all.
