# Time-series prediction in PyTorch 
### About:
This notebook is intended to be a beginner's introduction to predicting time-series data using some of PyTorch's simplest neural network building blocks. This guide came out of my need to use several channels of time-series data to predict a separate channel of a time-series output (i.e. a many-to-many prediction). Unfortunately, existing guides are either time-series forecasting (predicting how a time-series trend will evolve over time) or were too complex for a total beginner.   

The examples in this guide increase in complexity, but remain easy to visualize. If at times I am too verbose, it is out of an abundance of caution!!! 

### Requirements:
PyTorch build (1.7.1) for Python (I have v3.8.3). I used the Conda package.  
Installation details for PyTorch are here: https://pytorch.org/get-started/locally/  
Matplotlib and numpy will be needed.   
Sklearn is optional, but nice if you want to save some lines of writing a mean-squared-error calculation by hand.   
The guide is written as a jupyter notebook, which makes it easier for a beginner to track cause-and-effect.  
