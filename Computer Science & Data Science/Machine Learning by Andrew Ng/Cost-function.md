---
aliases: [Squared Error Function, Mean Squared Error]
---
## Cost-function
Date : 24-12-2021
tags: #ml, #ds

---

### Detail
Otherwise known as ==Squared Error Function== or ==Mean Squared Error==
The full formula is: $$J(\theta_0,\theta_1) = \frac{1}{2m}\sum_{i=1}^m(h_\theta(x^i)-y^i)^2 $$ where $$h_\theta(x) = \theta_0 + \theta_1x$$
![[Pasted image 20211224182032.png]]

Basically we want to minimize the $h_\theta(x)$ so that it should be as close to the real value as possible ($y^i$)

As $h_\theta(x)-y^i$ get closer to 0, that means the difference between our predicted value should be close to actual value.
It does that through minimizing the coefficient $\theta_0$ and $\theta_1$

In the picture, there's $1/2$ for the convenience in computing gradient descent, because the derivative of *square function* will cancel out the $1/2$ term.

More relating to Cost Function using contour graph explained by Andrew Ng on Coursera[^1]

### Reference
[^1]: [Cost Function - Intuition II | Coursera](https://www.coursera.org/learn/machine-learning/supplement/9SEeJ/cost-function-intuition-ii) 
[Cost Function | Coursera](https://www.coursera.org/learn/machine-learning/supplement/nhzyF/cost-function)