# Gradient_descent_daily_review

This is me before lunch break while I was listening to the lecture about Gradient descent.

![Gradient](https://github.com/parsakazempour/Gradient_descent_daily_review/blob/main/0%20BA_DE2Nr3Ohi5HhI.jpg)




This is also me after lunch break while I was trying to work on gradient descent repo!

![Gradient2](https://github.com/parsakazempour/Gradient_descent_daily_review/blob/main/jumping-out-of-window.gif)

















# Definition Of Gradient
A gradient measures how much the output of a function changes if you change the inputs a little bit." — Lex Fridman (MIT)




# What Is Gradient Descent in Machine Learning?

Gradient Descent is an optimization algorithm for finding a local minimum of a differentiable function. 
Gradient descent in machine learning is simply used to find the values of a function's parameters (coefficients) that minimize a cost function as far as possible.




# How Gradient Descent Works

Gradient descent is like hiking down to the bottom of a valley because it is a minimization algorithm that minimizes a given function.

The equation below describes what the gradient descent algorithm does:
b is the next position of our climber, while a represents his current position.
The minus sign refers to the minimization part of the gradient descent algorithm.
The gamma in the middle is a waiting factor and the gradient term ( Δf(a) ) is simply the direction of the steepest descent.




# Steps of Gradient Descent:

    Initialization:
        Start by initializing the model parameters randomly or with predefined values.
        Choose a learning rate (α), a crucial hyperparameter that determines the size of the steps taken during optimization.



    Forward Pass:
        Feed the input data through the model to obtain predictions.
        Compare the predictions to the actual values using a cost or loss function.



    Gradient Calculation:
        Compute the partial derivative of the cost function with respect to each model parameter. This gradient represents the direction of steepest ascent.



    Update Parameters:
        Adjust the model parameters in the opposite direction of the gradient to minimize the cost function.
        The update rule for each parameter θ is given by:
        θ=θ−α⋅∂J(θ)∂θθ=θ−α⋅∂θ∂J(θ)​
        where J(θ)J(θ) is the cost function.



    Repeat:
        Iterate steps 2-4 until the cost function converges to a minimum or a predetermined number of iterations is reached.



Formulas:

    Cost Function (J):
        The cost function measures the error between predicted and actual values.
        J(θ)=12m∑i=1m(hθ(x(i))−y(i))2J(θ)=2m1​∑i=1m​(hθ​(x(i))−y(i))2
        Here, hθ(x(i))hθ​(x(i)) is the model prediction for the ith example, y(i)y(i) is the actual value, and m is the number of examples.



    Gradient Descent Update Rule:
        The update rule for each parameter θ is given by:
        θ=θ−α⋅∂J(θ)∂θθ=θ−α⋅∂θ∂J(θ)​
        The partial derivative term represents the slope of the cost function with respect to each parameter.







# Types of Gradient Descent

There are three popular types of gradient descent that mainly differ in the amount of data they use: 





 
# Batch Gradient Descent

Batch gradient descent, also called vanilla gradient descent, calculates the error for each example within the training dataset, but only after all training examples have been evaluated does the model get updated. This whole process is like a cycle and it’s called a training epoch.

Some advantages of batch gradient descent are its computational efficiency: it produces a stable error gradient and a stable convergence. Some disadvantages are that the stable error gradient can sometimes result in a state of convergence that isn’t the best the model can achieve. It also requires the entire training dataset to be in memory and available to the algorithm.





 
# Stochastic Gradient Descent

By contrast, stochastic gradient descent (SGD) does this for each training example within the dataset, meaning it updates the parameters for each training example one by one. Depending on the problem, this can make SGD faster than batch gradient descent. One advantage is the frequent updates allow us to have a pretty detailed rate of improvement.

The frequent updates, however, are more computationally expensive than the batch gradient descent approach. Additionally, the frequency of those updates can result in noisy gradients, which may cause the error rate to jump around instead of slowly decreasing.





 
# Mini-Batch Gradient Descent

Mini-batch gradient descent is the go-to method since it’s a combination of the concepts of SGD and batch gradient descent. It simply splits the training dataset into small batches and performs an update for each of those batches. This creates a balance between the robustness of stochastic gradient descent and the efficiency of batch gradient descent.

Common mini-batch sizes range between 50 and 256, but like any other machine learning technique, there is no clear rule because it varies for different applications. This is the go-to algorithm when training a neural network and it is the most common type of gradient descent within deep learning.
