# Sign Language Alphabet Recognition
## Introduction
People always wonder what do each of the signs mean or what does the person who is unable to speak mean. One day while returning home from college I saw a person who was  interacting with another person in sign language and enjoying themselves. I started pondering as to what their actions mean and what they were trying to say. This drove me to create this project.
Sign Language is a unique type of communication that often goes understudied. While the translation process between signs and a spoken or written language is formally called ‘interpretation,’ the function that interpreting plays is the same as that of translation for a spoken language. In our research, we look at Indian Sign Language (ISL), which is used in the India and different countries have different gestures in their sign language. There are 22 handshapes that correspond to the 26 letters of the alphabet, and you can sign the 10 digits on one hand.

## Need of New System
The traditional system requires a person who knows and understands Sign Language and is able to translate it to regular speech for people to understand and for dumb and deaf people to understand our language as well. This is not always possible, hence this a new system is needed.

There is no such rock-solid approach currently implemented for translation of Sign Language to English alphabets and there are a few projects and papers of the same. So the current project has to be capable of translating a few characters with some amount of accuracy.

## Dataset
The dataset used in this project is an augmented version of the dataset from https://github.com/imRishabhGupta/Indian-Sign-Language-Recognition . For augmenting the dataset, I have taken help of a script from the linked project.

For training the model, I have used the dataset with 3983 images and 24 classes. It contains images of signs for each alphabet from A-Z except J and Z since both of them require temporal data as well which this current model is incapable of doing. Hence, we only have 24 classes instead of 26 classes.

This project was created and trained on google colab with dataset uploaded on google drive

## Model
This model was trained on the dataset containing 3983 images belonging to 24 unique classes and 985 images were used to evaluate the model. The model was built using the TensorFlow Framework. The model that is created is a CNN model(Convolutional Neural Network) which is used for image classification.

The architecture of the model consists of two Convolutional 2D layers, two Max Pooling 2D layers, one Flatten layer and two Dense layers.

All the pre-processed images are sent to the input layer.

## Predicting for New Images
New images cannot be directly sent for prediction. They must first undergo the preprocessing step. Then the image can be sent to the model for prediction. The accuracy of the prediction for new images completely depends on how well the image gets pre-processed.

## Conclusion
If the pre-processing of the image has some major redundancies, then the answer may or may not vary from the desired result.

Hence to obtain good results, use an image with a plain background preferably white background.

## About Me
I am an Engineering Student who recently found his interest in Deep Learning, ML, AI. This is my first Deep Learning Project apart from the one's I've done while learning a course.
