## Gradient Descent
Date : 24-12-2021
tags: #ml, #ds

### Detail

#### Basic
We graph the hypothesis function base on $\theta_0$ and $\theta_1$ on z, x and y axis respectively. We get the following graph.

![[Pasted image 20211224233717.png]]

Where the points will be the result of the cost function using hypothesis with different theta parameters.

We aim to minimize our hypothesis function, which ideal value would be at the bottom (minimum value).

To find the minimized value, we do this by taking derivative of our cost function. The slope of the tangent is the derivative of that point and it shows us which direction to move towards to achieve optimal decrease in $J(\theta_0,\theta_1)$ per step.

The size of each step taken is determined through *learning rate*, denoted by $\alpha$ . Each step are shown as **X** in the graph.

The gradient descent algorithm is as followed: $$\theta_j \coloneqq \theta_j - \alpha\frac{\partial}{\partial\theta_j}J(\theta_0,\theta_1)$$ 
where j=0,1 represents feature index number from the hypothesis function formula. The formula above should be repeated until converge at minimum point. 

At each iteration *j*, each parameter should be updated simultaneously. 

![[Pasted image 20211224235148.png]]

#### Example with single parameter

Try formula for single parameter: $$\theta_1 \coloneqq \theta_1 - \alpha\frac{\partial}{\partial\theta_1}J(\theta_1)$$

![[Pasted image 20211225004003.png]]

It will converge to minimum value regardless of the derivative sign. If derivative is positive slope, $\theta_1$ will move backward and vice-versa.

We should adjust our learning-rate $\alpha$ to make sure the gradient converges in a reasonable time while not over-stepping.

![[Pasted image 20211225004201.png]]

With learning ratee $\alpha$ fixed, gradient descent will still converge to local minimum. At the minimum the derivative will be 0, therefore: $$\theta_1 \coloneqq \theta_1 - \alpha*0$$

![[Pasted image 20211225004400.png]]


### Reference
[Gradient Descent Intuition | Coursera](https://www.coursera.org/learn/machine-learning/supplement/QKEdR/gradient-descent-intuition)