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


# 1. Initialization:

    Initialize model parameters θθ randomly or with some predefined values.
    Choose a learning rate (αα).

# 2. Calculate the Cost Function:

    Calculate the cost function J(θ)J(θ) for the current parameters.
    The cost function measures the difference between predicted and actual values.

# Formula:
J(θ)=12m∑i=1m(hθ(x(i))−y(i))2J(θ)=2m1​∑i=1m​(hθ​(x(i))−y(i))2

where:

    mm is the number of training examples.
    hθ(x(i))hθ​(x(i)) is the predicted output for input x(i)x(i).
    y(i)y(i) is the actual output.

# 3. Calculate the Gradient:

    Compute the gradient of the cost function with respect to each parameter.

Formula:
∂J(θ)∂θj=1m∑i=1m(hθ(x(i))−y(i))⋅xj(i)∂θj​∂J(θ)​=m1​∑i=1m​(hθ​(x(i))−y(i))⋅xj(i)​

for each parameter θjθj​.

# 4. Update Parameters:

    Update each parameter using the gradient and the learning rate.

Formula:
θj=θj−α∂J(θ)∂θjθj​=θj​−α∂θj​∂J(θ)​

for each parameter θjθj​.

# 5. Repeat:

    Repeat steps 2-4 until convergence or a predefined number of iterations.



# 6. Predict:

    Use the trained model with the final parameters to make predictions on new data.

This flowchart provides a high-level overview of the gradient descent algorithm.
Remember that the success of gradient descent depends on the appropriate choice of the learning rate and the characteristics of the cost function.
Adjustments may be needed based on the specific requirements of your problem.
