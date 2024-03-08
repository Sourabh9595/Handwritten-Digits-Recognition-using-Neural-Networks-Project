Index

1.	Introduction	
2.	Methodology	
3.	Conclusion	



Introduction
In this experiment, the task involved creating different ANN model architectures and training them with a dataset to see how they behave. The dataset is composed of handwritten images stored as 32 * 32 matrix pixels, with each pixel taking a value of 1 or 0 corresponding t black and white pixels.  Each file had one data example per line. So each line consisted of 1025 space-separated integers. This is 1024, 32 * 32 features and one label indicating which number is represented by the stream. With this dataset, the neural networks were supposed to have different architectures. These architectures are described as:
. A (multi-output) perceptron with 1024 input units and 10 output units, with (gradient descent) learning rate ∈ {4 i |i = 0, 1, 2, 3, 4}, at least
 A deep neural network with the same number of units per hidden layer ∈ {4^2 , 4^3 , 4^4}, network depth (i.e., number of hidden layers) ∈ {1, 2, 3, 4}, and (gradient descent) learning rate ∈ {4 i |i = −2, −1, 0, 1, 2}, at least 
 A deep neural network with 2 hidden layers, with the number of units in the first layer ∈ {4^3 , 4^4} (connecting from the input layer), followed by a smaller number of units ∈ {4^2 , 4^3} in the next layer (connecting to the output layer), and (gradient descent) learning rate ∈ {4 i |i = −3, −2, −1, 0, 1}, at least
All the neural networks were sigmoid. Using cross-validation of 3, the best model would be chosen.


Methodology
I used the neural network architectures described in the introduction section. From each of the architectures, several parameters were used and several outputs were of interest. I started by defining the first mode. The model used a single input layer and an output layer. 
The input layer had 1024 neurons while the output layer had 10 neurons. This represents the inputs and the inputs respectively. 
Second, I prepared the data for training the model. Since the data was in DAT files, I loaded the data. I then split the lines to obtain each value as a single part of a column. The labels, which were the last value in each line of data had to be converted to categorical data for easy use in the model. 
After the data pre-processing, I fitted the model and started to gather the requirements from the model. From the model, I recorded the values of the training and test proxy error function and the training and test misclassification and plotted the errors as required.
The second task I did with the models is to tabulate and visualize the average CV test misclassification.
The third thing I did with the model is to plot the gradient descent fitting curves.
I did this for the three model architectures.


Conclusion
In conclusion, we see that the model architecture is a factor in the output we get from a model. The output in this case is in the form of error rates and accuracy. Although we have used cost functions in the model, using utility functions would lead to the same results 
of increasing accuracy with better models. However, it is not definitive about the type of model to use. As seen from the models, the second architecture has the fewest errors, even though it is not the most complex. Another factor that affects the learning and the 
results of a model is the number of examples used. As the number of instances increases, the better the model.

