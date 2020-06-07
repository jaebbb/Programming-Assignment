## Prerequisite
- Programming Language: I recommend the Python language but you can use any kind of programming languages. e.g. Matlab, C, C++, JAVA ....  
- Do not use any deep learning frameworks. e.g. PyTorch, Tensorflow, Keras, ...  
- Do not use GPU-based implementations.  
- Submit your code in a “.zip” file, and submit your report (“.pdf” file) to explain kindly your implementation and to discuss your results. (Due: 11:59pm, 02-June-2020)  
- Putting comments in your code.  

## Task 0. Generate randomly 2-dimensional training / test data (10 pt)  
The number of classes is 2, and the target label is one-hot encoded code (e.g. [1 0] for 1st class and [0 1] for 2nd class). 
The training data of the first class are drawn from Gaussian distribution with μ = [1 1], Σ = [1 0; 0 1] (Identity matrix). 
Also, for the second class, the training data are drawn from Gaussian distribution with μ = [−1 − 1], Σ = [1 0; 0 1].  
Generate test data which are drawn from the same distribution for each class. The number of training data is 100, and the number of test data is 100.  

## Task 1. Build the fully connected layer model. (20 pt)  
Input layer (2) -> Fully connected layer (10) -> ReLU -> Fully connected layer (10) -> ReLU -> Fully connected (output) layer (2) , where (·) denotes the number of nodes.  
Just initialize the weights randomly with Gaussian distribution with μ = 0, σ = 0.001. Task 2. Implement Forward Pass of the Network (20 pt)  

## Task 2. Implement Forward Pass of the Network (20 pt)  
Perform forward pass (inference) using the test data without any training process. Calculate the accuracy as follows:
```
Accuracy = The Number of Correct Samples/Total Number of Data Samples ∗ 100 (%) (1)
```  

## Task 3. Implement Backward Pass of the Network (50 pt)  
Update the weights of your network using the stochastic gradient descent method. Use MSE (mean squared error) loss, and you don’t need to use softmax function. Calculate the accuracy of the network and compare it with the accuracy in Task 2.  
(Hint: You need to calculate gradients. You can use any batch size. e.g. 1)  
