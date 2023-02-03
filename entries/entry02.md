# Entry 2
##### 12/14/2022

# Neural Network

While starting out, I thought that training a neural network would be as easy as just feeding it a set of information and it would just learn based on the dataset that it was fed. But after starting, I realized that there are so many different factors that are involved with a neural network. There are steps like normalizing the data which confused me at first. There are concepts that I have to learn like creating a training set and a verification set. The training set is used for training the machine learning model, and the verification set is used to ensure that the trained machine learning model understands how to intepret data that it has never seen before. Even beyond the concepts, there are functions that are used to train the machine learning model. There are optimizer functions such as Adam, Stochastic Gradient Descent (with momentum), Adagrad, RMSProp, AdaDelta, Mini-Batch Gradient Descent, and just Gradient Descent. For mine, I found Stochastic Gradient Descent to work best with what I'm trying to do with my machine learning model.

# HTTP Server and Client

To get the Arduinos on the gloves to report data to the computer, where it would be interpreted, I would have to set up a basic HTTP server so that it could communicate with any server remotely. To do this, I researched basic HTTP servers in Python, where I happened to stumble across Flask. I would then use the data reported to the HTTP server and store it in a new row in a CSV file. This is then combined with all the CSV files with data from both hand to train the neural network. But before this, I also have to get the Arduino to work as a HTTP client. To do this, I had to connect the Arduino to a WiFi network, then I had to include all the sensor readouts from the ADC0 pins in an array. After this, I send the array to the HTTP server via a HTTP PUSH request. Using that, I store all of it to the CSV file by using the writer function built into the CSV library/API. This data would later be used to train the neural network.

# Learning Sources

freeCodeCamp is a great source for everything that involves programming. To start, I started by searching for basic [text classification videos for TensorFlow](https://www.youtube.com/watch?v=VtRLrQ3Ev-U). She goes over basically all the concepts that I have used to classify text. By following this tutorial, I was able to create a training dataset and a validation dataset for my neural network. As explained in the video, the training dataset is used to make sure that the model understands what it is looking at, but the validation dataset is used to make sure that the model can understand new data. As a proof of concept, I only trained it on the first 3 characters of the alphabet. Results were mixed because of the inaccuracy of the flex sensors.

# Engineering Design Process

I would say I'm somewhere between plan the most promising solution and create a prototype. I am still trying to sort out how I should approach a larger set of words to translate. 

# Skills

The skills that I am applying are Problem Decomposition, How to Learn, and How to Google.


[Previous](entry01.md) | [Next](entry03.md)

[Home](../README.md)
