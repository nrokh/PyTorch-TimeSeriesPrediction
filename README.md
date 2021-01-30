# A guide to time-series prediction in PyTorch 
### About:
This notebook is intended to be a beginner's introduction to predicting time-series data using some of PyTorch's simplest neural network building blocks. This guide came out of my need to use several channels of time-series data to predict several different channels of a time-series output (i.e. a many-to-many prediction). Unfortunately, existing guides are either time-series forecasting (predicting how a single time-series trend will evolve over time), were classification problems instead of regression, or were too complex for a beginner. I am assuming that the reader of this guide is familiar with the concepts of supervised learning, forward and backward propagation, gradient descent, linear algebra. I'd love to teach you the content of an entire machine learning course in one simple guide, but I can't yet.  

The examples in this guide increase in complexity, but remain easy to visualize. If at times I am too verbose, it is out of an abundance of caution!!! 

### Requirements:
PyTorch build (1.7.1) for Python (I have v3.8.3). I used the Conda package.  
Installation details for PyTorch are here: https://pytorch.org/get-started/locally/  
Matplotlib and numpy will be needed.   
Sklearn is optional, but nice if you want to save some lines of writing a mean-squared-error calculation by hand.   
The guide is written as a jupyter notebook, which makes it easier for a beginner to track cause-and-effect.  

### Overview:
I am assuming that the reader of the guide is familiar with the concepts of supervised learning, forward and backward propagation, gradient descent. 
This guide consists of 5 examples:  
1. Using one continous signal to predict another using a fully-connected network with 3 linear layers
2. Training the model from Ex.1 with several batches of input data
3. Modifying the model from Ex.1 to accept an input of 2 continous signals in each sample
4. Modifying the model from Ex.3 to output 2 continous signals 
5. Using dropout as one way to prevent overfitting  

I'm working on an extension to this guide that will include similarly simple examples of convolutional layers and maybe even an LSTM implementation if I can figure out how windowing works. 
