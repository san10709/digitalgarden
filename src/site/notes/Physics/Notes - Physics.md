---
{"dg-publish":true,"permalink":"/physics/notes-physics/"}
---

[[IFSS\|IFSS]]
# Detailed Comments
## General Relativity
### 1. Schutz 2e[ ](<D:\Knowledge\BOOKS\Physics\Advanced Physics\General Relativity\A First Course in General Relativity 2e - Schutz.pdf>)
###### 15. Page 74
Remember, the order of the indices of $\eta$ doesn't matter since it's symmetric. So the way to raise/lower an index is simply to introduce an $\eta$ and sum over that index (which means that we'll be summing over only one index of $\eta$).
###### 14. Page 72
For every vector $\mathbf{v}\in V$ we can construct the unique one-form $\tilde{p}\in V^*$ using the metric tensor such that $\tilde{p} = \mathbf{g}(\mathbf{v},\;\;)$ and in this way we can construct all the one-forms in $V^*$. Now we shift our focus to a specific vector, $\mathbf{w}$, and view it as a (linear) function of the one-forms into the real numbers: $\mathbf{w}:V^*\longrightarrow \mathbb{R}$ such that 
$$\large{\mathbf{w}(\tilde{p}) = \mathbf{g}(\mathbf{v},\mathbf{w}) = \tilde{p}(\mathbf{w})}$$
So $\mathbf{w}$ is simply filling in the empty slot of $\large\tilde{p}$. Note that the contraction, $p_\alpha V^\alpha = \eta_{\alpha \beta}p^\beta V^\alpha$, is actually a scalar product. 
###### 13. Page 71
The motivation/rationale for defining the magnitude, and hence the scalar product, of one-forms can be understood as follows: consider the magnitude of a vector, $\vec{p}^{\;2}=\eta_{\alpha \beta}p^\alpha p^\beta = \eta_{\alpha \beta}\left(\eta^{\alpha \mu} p_\mu\right)\left(\eta^{\beta \nu} p_\nu\right) =\eta^{\alpha \mu} p_\mu p_\alpha$. Now, the leftmost expression contains the metric and only the components of the vector $\vec{p}$ obtained from the one-form $\large\tilde{p}$ and the rightmost expression contains the inverse metric and only the components of the one-form $\large\tilde{p}$, and these two expressions are equal. It makes sense to define the magnitude of the one-form as the later. 
###### 12. Page 70
We know that $\large\tilde{d}\phi = \mathbf{g}(\vec{d}\phi,\;\;)$ so $\large\tilde{d}\phi(\vec{V})=\mathbf{g}(\vec{d}\phi,\vec{V})=\vec{d}\phi\cdot\vec{V}$. However, it's not trivial to say that $\large\tilde{d}\phi(\vec{V})$ is the rate of change of $\phi$ along $\vec{V}$ because that's true only when $\vec{V}$ is a tangent vector so that its components are $dx^\alpha/d\tau$ and we have: $$\large\tilde{d}\phi(\vec{V}) = \tilde{d}\phi_\alpha V^\alpha = \frac{\partial \phi}{\partial t}\frac{\partial t}{\partial \tau}+\frac{\partial \phi}{\partial x}\frac{\partial x}{\partial \tau}+\frac{\partial \phi}{\partial y}\frac{\partial y}{\partial \tau}+\frac{\partial \phi}{\partial z}\frac{\partial z}{\partial \tau} = \frac{d\phi}{d\tau}$$
What if the vector is not a tangent vector?
###### 11. Page 56
We can convert the set of all $\binom{0}{N}$ tensors into a vector space by defining the addition and scalar multiplication of these tensors as follows: Let $T_1$ and $T_2$ be two $\binom{0}{N}$ tensors then we define $T_3=T_1+T_2$ such that
$$T_3(\vec{A}_1,\cdots,\vec{A}_N)=T_1(\vec{A}_1,\cdots,\vec{A}_N)+T_2(\vec{A}_1,\cdots,\vec{A}_N)$$ and $R=\alpha T$ such that $R(\vec{A}_1,\cdots,\vec{A}_N)=\alpha[T(\vec{A}_1,\cdots,\vec{A}_N)]$ 
###### 10. Page 64
This needs a bit explaining: we're here talking about changing basis. Remember the equivalent ways of looking at 4-tuples; as coordinates of events/points and as the components of position vectors of those events/points. When we choose a basis it defines coordinates for each event/point in that space. So changing basis means the coordinates assigned to each event/point also change. $\phi$ which was initially a function of $t,x,y,z$ is now a function of $\bar{t},\bar{x},\bar{y},\bar{z}$. So

$$\large{
\begin{align}
\frac{\partial \phi}{\partial \bar{t}} &= \frac{\partial \phi}{\partial t}\frac{\partial t}{\partial \bar{t}}\\
\Longrightarrow
\frac{\partial \phi}{\partial x^{\large\bar{\alpha}}} &= \frac{\partial \phi}{\partial x^{\alpha}}\frac{\partial x^{\alpha}}{\partial x^{\large\bar{\alpha}}}
\end{align}}$$


###### 9. Page 56
A tensor of type $\binom{0}{N}$ is a multilinear function (linear in each of its arguments) of $N$ vectors into the real numbers:$$\begin{gather}T:\underbrace{V\times \cdots\times V}_N \longrightarrow\mathbb{R}\\\\
T(\cdots,\alpha v_1+\beta v_2,\cdots)=\alpha T(\cdots,v_1,\cdots)+\beta T(\cdots,v_2,\cdots)
\end{gather}$$
###### 8. Page 47
Don't be too confused about the meaning/interpretation of $d^2\vec{x}$ and $d\tau^2$: their meanings were unclear when we considered the second derivative in calculus too 😃. Understand $\frac{d\vec{U}}{d\tau}$ as the scalar $\frac{1}{d\tau}$ being multiplied with a vector $d\vec{U}$ which is formed by changing the components of $\vec{U}$ infinitesimally.
###### 7. Page 21
The $\bar{t}$-axis has a slope of $1/v$ and passes through the origin so its equation is $t=(1/v)x\Longrightarrow vt-x=0$. Similarly, the $\bar{x}$-axis has a slope of $v$ and passes through the origin so its equation is $t=vx\Longrightarrow vx-t=0$. Putting $\bar{x}=0$ (the $\bar{t}$-axis) in $\bar{x}=\gamma t + \sigma x$ gives $-\sigma/\gamma=1/v\Longrightarrow \gamma/\sigma=-v$, and putting  $\bar{t}=0$ (the $\bar{x}$-axis) in $\bar{t}=\alpha t + \beta x$ gives $\beta/\alpha=-v$.
###### 6. Page 19
The definition of $\Delta s^2$ comes from the speed of light being equal to $1$:
$$\begin{align}c &= \frac{\text{distance}}{\text{time}}\\
1 &= \frac{\sqrt{(\Delta x)^2+(\Delta y)^2+(\Delta z)^2}}{\Delta t}\\
1^2 &= \frac{(\Delta x)^2+(\Delta y)^2+(\Delta z)^2}{(\Delta t)^2}\\
(\Delta t)^2 &= (\Delta x)^2+(\Delta y)^2+(\Delta z)^2\\
0 &= -(\Delta t)^2 + (\Delta x)^2+(\Delta y)^2+(\Delta z)^2  \tag{1}\\
(\Delta t)^2 &- (\Delta x)^2 - (\Delta y)^2 - (\Delta z)^2 = 0  \tag{2}\end{align}$$
That's why we can define $\Delta s^2$ either with $(1)$ or with $(2)$.
###### 5. Page 18
We have:$$\begin{align}\Delta \bar{s}^2_{AC} &= -(\bar{t}_C - \bar{t}_A)^2 + (\bar{x}_C - \bar{x}_A)^2\\
&= -0+l^2 = l^2\\
\Delta s^2_{AC} &= -(t_C - t_A)^2 + (x_C - x_A)^2\\
&= -t^2_C + x^2_C\end{align}$$
Since the interval is invariant, and the event $C$ lies on the $\bar{x}$-axis which means that $v=t_C/x_C$, we have
$$\begin{align}-t^2_C + x^2_C &= l^2\\
-(vx_C)^2+x^2_C &= l^2\\
x_C &= \frac{l}{\sqrt{1-v^2}}\end{align}$$
###### 4. Page 17-2
The event $B$ lies on the $\bar{t}$-axis and the hyperbola $-t^2+x^2=-1$ so we have
$$\begin{align} \frac{1}{v} &= \frac{t}{x}\qquad \text{and}\qquad -t^2+x^2=-1\\
\Rightarrow x &= vt \qquad \Rightarrow\qquad -t^2+(vt)^2=-1\\
t^2(1-v^2) &= 1\\
t &= \frac{1}{\sqrt{1-v^2}}\end{align}$$
###### 3. Page 17-1
An alternate way to view this problem is to think of the $xt$-axes and the $\bar{x}\bar{t}$-axes as two sets of bases vectors for this 2D space: how do we find all the points with $t=\text{constant}$, we draw a line parallel to the $x$-axis through $t=\text{constant}$. Similarly, how do we find all the points with $\bar{t}=\text{constant}$, we draw a line parallel to the $\bar{x}$-axis through $\bar{t}=\text{constant}$. Now we've to show that the tangent to a hyperbola at a point, $P$, is a line of simultaneity for a frame whose $t$-axis passes through that point, $P$. Since nothing can move faster than light, the $\bar{t}$-axis of an observer is always timelike so we should focus on evets/points on the hyperbola, $-t^2+x^2=-b^2$. The slope of the tangent is: $$\begin{align}t^2 &= x^2+b^2\\
\frac{dt}{dx} &= \frac{x}{t}\end{align}$$
For a point $P$ with coordinates $(x_0,t_0)$ the slope of the tangent line will be $x_0/t_0$. Now imagine we draw a $\bar{t}$-axis through the origin and $P$. The slope of this line will be $t_0/x_0$ and so the slope of its $\bar{x}$-axis will be $x_0/t_0$. Hence the $\bar{x}$-axis and the tangent of the hyperbola are parallel.
###### 2. Page 9
The speed of light being $1$ means:
$$\begin{align}c &= \frac{\text{distance}}{\text{time}}\\
1 &= \frac{\sqrt{(\Delta x)^2+(\Delta y)^2+(\Delta z)^2}}{\Delta t}\\
1^2 &= \frac{(\Delta x)^2+(\Delta y)^2+(\Delta z)^2}{(\Delta t)^2}\\
(\Delta t)^2 &= (\Delta x)^2+(\Delta y)^2+(\Delta z)^2\\
0 &= -(\Delta t)^2 + (\Delta x)^2+(\Delta y)^2+(\Delta z)^2\end{align}$$
###### 1. Page 4
You can understand the conversion to these 'natural' units like this: the speed of anything is most generally defined as:
$$\text{v} = \frac{\text{distance traveled in a given time interval}}{\text{that given time interval}}$$
Normally, we take the time interval to be $1\text{s}$, but we don't have to! In this particular case where we want to make $c$ have a magnitude of $1$, we choose it to be $(3\times 10^8)^{-1} \text{s}$ and call it $1$ meter of time: we can call it something else, but this reduces the dimensions of many quantities whenever speed (m/s) appears.
Note that we could have very well redefined $3\times 10^8 \text{m}$ to be $1$ second of distance, which is actually the definition of light second.
### 2. Carroll[ ](<D:\Knowledge\BOOKS\Physics\Advanced Physics\General Relativity\Spacetime and Geometry - Sean Carroll.pdf>)
###### 3. Page 61
Note that the order doesn't matter: $\phi_1\circ \phi_2^{-1}=\left(\phi_2\circ \phi_1^{-1}\right)^{-1}$.
###### 2. Page 62
Since points on the sphere in the region $-1<x^3<1$ are given the coordinates $(y^1,y^2)$ and $(z^1,z^2)$ so a transformation/equation that gives one of these in terms of the others is changing of coordinates.
###### 1. Page 60
All $n$-dimensional manifolds can be embedded in $\mathbb{R}^{2n}$ but it's not necessary for every $n$-dimensional manifold to be embeddable in $\mathbb{R}^m$ with $n\le m\le 2n$.
### 3. Schutz[ ](<D:\All\Downloads\Geometrical Methods of Mathematical Physics - Schutz.pdf>)
###### 1. Page 131
On an $n$-dimensional manifold a $p$-form has $n!/(n-p)!p!$ independent components and hence the vector space it makes has this dimension: when $p=n$ this is a one dimensional vector space.
## Computational Physics
### 1. Numerical Methods in Physics with Python - Gezerlis
###### 3. Page 460
Small values of $X$ give gross overestimations of the integral and larger values give gross underestimations of the integral. Since in Monte-Carlo quadrature we're averaging these estimates doesn't it make sense to pick these points *uniformly* so that we're as likely to overestimate it as we are to underestimate it? Picking these random points exponentially means we'll be more often overestimating the integral and hence their average (in Monte-Carlo quadrature formula) will also be an overestimation, right?

| Underestimation                      | Overestimation |
| ------------------------------------ | -------------- |
| ![Pasted image 20230806222310.png](/img/user/Attachments/Pasted%20image%2020230806222310.png) | ![Pasted image 20230806222322.png](/img/user/Attachments/Pasted%20image%2020230806222322.png)               |

###### 2. Page 473-2
Note that for a random variable $X$ with probability density function $p(x)$, a function of it is another random variable, $f(X)=Y$, and its density function, $q(y)$, is generally different from $p(x)$. Now, the expectation of a random variable is defined as $E[Y]=\int yq(y)dy=\int f(x)q(y)dy$ but we're claiming that this is equal to $\int f(x)p(y)dy$ ($y$ and and $x$ are just dummy variables): note that this does not imply that $p(x)=q(x)$ since the integrals being equal only means that the areas under their graphs are equal. The resolution of this is that there is a theorem that proves this:
![Pasted image 20230806225911.png](/img/user/Attachments/Pasted%20image%2020230806225911.png)
###### 1. Page 473-1
Consider a single random variable $X$ with density $p(x)$ and another random variable $Y=f(X)$ with density $p_Y(y)$. We make $n$ measurements of $X$ and get the realizations $x_0,x_1,...,x_{n-1}$ and find the corresponding values of $Y$ using $f(x)$. Now we compute the arithmetic mean of these values: $$\large{\bar{f}=\frac{1}{n}\sum_{i=0}^{n-1}{f(x_i)}}$$
We claim that $\bar{f}$ is also a random variable (a random variable is a quantity whose repeated measurements yield outcomes based on a probability density): measuring $\bar{f}$ again means that we've to make $n$ measurements of $X$ again which will yield different numbers than our initial sample $(x_0,x_1,...,x_{n-1})$ and hence the value of $\bar{f}$ will also change. Now we *propose* a different definition of $\bar{f}$ and hence a different way to look at this random variable: take $n$ random variables $X_0,X_1,...,X_{n-1}$ all having the same probability density function $p(x)$. For a function or a transformation $f$ , $f(X_0),f(X_1),...,f(X_{n-1})$ are also random variables. A linear combination of random variables is also a random variable so define
$$\large{\bar{f}=\frac{1}{n}\sum_{i=0}^{n-1}{f(X_i)}}$$
A measurement of $\bar{f}$ means a *single* measurement of each $X_i$. And using the facts that $E[kX]=kE[X]$ and $E[\sum X_i]=\sum E[X_i]$ we get:
$$\large{E[\bar{f}]=\frac{1}{n}\sum_{i=0}^{n-1}{E[f(X_i)]}=\frac{1}{n}\sum_{i=0}^{n-1}{\int f(x)p(x)dx}=\frac{1}{n}\sum_{i=0}^{n-1}{\langle f(X)\rangle}=\langle f(X)\rangle}$$
Since each of the $X_i$'s have the same density $p(x)$ their expectations are the same.

References:
- [https://www.probabilitycourse.com/chapter7/7_1_1_law_of_large_numbers.php](https://www.probabilitycourse.com/chapter7/7_1_1_law_of_large_numbers.php)
- [https://www.math.wichita.edu/~cma/stat774/ch3.pdf](https://www.math.wichita.edu/~cma/stat774/ch3.pdf)
- [https://www.scratchapixel.com/lessons/mathematics-physics-for-computer-graphics/monte-carlo-methods-mathematical-foundations/expected-value.html](https://www.scratchapixel.com/lessons/mathematics-physics-for-computer-graphics/monte-carlo-methods-mathematical-foundations/expected-value.html)
- [https://www.scratchapixel.com/lessons/mathematics-physics-for-computer-graphics/monte-carlo-methods-in-practice/monte-carlo-integration.html](https://www.scratchapixel.com/lessons/mathematics-physics-for-computer-graphics/monte-carlo-methods-in-practice/monte-carlo-integration.html)
### 2. Andrew Ng Notes[ ](<D:\Knowledge\BOOKS\Physics\Computational Physics\Machine Learning\Andrew Ng Notes.pdf>)
###### 18. Page 

###### 17. Page 89
Let's vectorize the two-layer fully-connected neural network over the training examples.
Let us have $n$ examples with $d$ features and $m$ neurons in the hidden layer. For a single example, we can vectorize the whole hidden layer like this:
$$\underbrace{\begin{bmatrix}z_1\\ \vdots \\ z_m\end{bmatrix}}_{\Large z\in\mathbb{R}^{m\times 1}} = \underbrace{\begin{bmatrix}\textemdash\left(w_1^{[1]}\right)^\intercal\textemdash\\ \vdots \\ \textemdash\left(w_m^{[1]}\right)^\intercal\textemdash \end{bmatrix}}_{\Large W^{[1]}\in\mathbb{R}^{m\times d}}\;
\underbrace{\begin{bmatrix}x_1\\ \vdots \\ x_d\end{bmatrix}}_{\Large x\in\mathbb{R}^{d\times 1}} + 
\underbrace{\begin{bmatrix}b^{[1]}_1\\ \vdots \\ b^{[1]}_m\end{bmatrix}}_{\Large b^{[1]}\in\mathbb{R}^{m\times 1}}$$
and then $a=\text{ReLU}(z)$ is defined element-wise. and defining $W^{[2]}=\left(w^{[2]}\right)^\intercal \in \mathbb{R}^{1\times m}$ and $b^{[2]}\in\mathbb{R}$ we have
$$h_\theta(x)=W^{[2]}a+b^{[2]}$$
To vectorize over all the examples, we can construct our design matrix $X$ to have each example along a column making it $d\times n$, then $z$ becomes $m\times n$, and $a$, defined element-wise, also becomes $m\times n$. $W^{[2]}$ is still $1\times m$ but $b^{[2]}$ is now $1\times n$ so $h_\theta(x)$ is also $1\times n$.
###### 16. Page 101
1. Let's verify line 4 in Algorithm 5:
   $$\begin{align}
   \mathbf{a}^{[k]} &= \text{ReLU}(\mathbf{z}^{[k]}) \\
   J &= J(\mathbf{a}^{[k]}) \\
   \frac{\partial J}{\partial \mathbf{z}^{[k]}} &= \frac{\partial J}{\partial \mathbf{a}^{[k]}} \odot\text{ReLU}'(\mathbf{z}^{[k]})\tag{1} &&\text{(using eq. 7.41)}
   \end{align}$$
   We also have
   $$\begin{align}
   \mathbf{z}^{[k+1]} &= \text{W}^{[k+1]}\mathbf{a}^{[k]} + b^{[k+1]} \\
   J &= J\big(\mathbf{z}^{[k+1]}\big)
   \end{align}$$
   Then from equation 7.38 we have
   $$\begin{align}
   \frac{\partial J}{\partial \mathbf{a}^{[k]}} &= \left(\text{W}^{[k+1]}\right)^\intercal \frac{\partial J}{\partial \mathbf{z}^{[k+1]}}\\
   &= \left(\text{W}^{[k+1]}\right)^\intercal\boldsymbol{\delta}^{[k+1]}
   \end{align}$$
   So $(1)$ becomes
   $$\boxed{
   \frac{\partial J}{\partial \mathbf{z}^{[k]}} = \big(\text{W}^{[k+1]}\big)^\intercal\boldsymbol{\delta}^{[k+1]} \odot\text{ReLU}'\left(\mathbf{z}^{[k]}\right)}$$
2. Let's verify the equations in line 5 of Algorithm 5:
   $$\begin{align}
   \mathbf{z}^{[k+1]} &= \text{W}^{[k+1]}\mathbf{a}^{[k]} + b^{[k+1]} \\
   J &= J\big(\mathbf{z}^{[k+1]}\big)
   \end{align}$$
   Then from equation 7.39 we have
   $$\boxed{
   \frac{\partial J}{\partial \text{W}^{[k+1]}} = \boldsymbol{\delta}^{[k+1]}\cdot\left(\mathbf{a}^{[k]}\right)^\intercal}$$
   And
   $$\boxed{
   \frac{\partial J}{\partial b^{[k+1]}} = \boldsymbol{\delta}^{[k+1]}}$$
###### 15. Page 100-2
1. Let's verify the first equation in line 4 in Algorithm 4:
   $$\large\begin{align}
   o &= \text{W}^{[2]}\mathbf{a} + b^{[2]} \\
   J &= J(o)
   \end{align}$$
   Then from equation 7.39 we have
   $$\large\begin{align}
   \frac{\partial J}{\partial W^{[2]}} &= \frac{\partial J}{\partial o}\mathbf{a}^\intercal &&\left(\text{since }\frac{\partial J}{\partial o} \text{ is a scalar}\right)\\
   &= (o-y)\mathbf{a}^\intercal\\
   &= \delta^{[2]}\mathbf{a}^\intercal
   \end{align}$$
2. Let's verify the second equation in line 4 in Algorithm 4: 
   $$\large\begin{align}
   o &= \text{W}^{[2]}\mathbf{a} + b^{[2]} \\
   J &= J(o)
   \end{align}$$
   Then from equation 7.40 we have
   $$\large\begin{align}
   \frac{\partial J}{\partial b^{[2]}} &= \frac{\partial J}{\partial o}\\
   &= (o-y)\\
   &= \delta^{[2]}
   \end{align}$$
3. Let's verify the forth equation in line 4 in Algorithm 4: 
   $$\large\begin{align}
   \mathbf{z} &= \text{W}^{[1]}\mathbf{x} + b^{[1]} \\
   J &= J(\mathbf{z})
   \end{align}$$
   Then from equation 7.40 we have
   $$\large\begin{align}
   \frac{\partial J}{\partial b^{[1]}} &= \frac{\partial J}{\partial \mathbf{z}}\\
   &= (o-y)\cdot W^{[2]}\odot\text{ReLU}'(\mathbf{z})\\
   &= \delta^{[1]}
   \end{align}$$
###### 14. Page 100-1
Note that we have for a two-layer neural network:
$$\large\begin{align}
\mathbf{z} &= \text{W}^{[1]}\mathbf{x}+\mathbf{b} \\
\mathbf{a} &= \text{ReLU}(\mathbf{z}) \\
o &= \text{W}^{[2]}\mathbf{a} + b^{[2]} \\
J &= \frac{1}{2}(y-o)^2
\end{align}$$
So $J$ is a function of $\mathbf{z}$ in a complicated way (through $o\rightarrow \mathbf{a}\rightarrow \mathbf{z}$). So we can write
$$\large\begin{align}
\mathbf{z} &= \text{W}^{[1]}\mathbf{x}+\mathbf{b} \\
J &= J(\mathbf{z})
\end{align}$$
And hence use equation 7.39 to find
$$\large
\frac{\partial J}{\partial \text{W}^{[1]}} = \frac{\partial J}{\partial \mathbf{z}}\cdot \mathbf{x}^\intercal$$

###### 13. Page 97
Each $\large\frac{\partial J}{\partial z_j}$ is common to all the components of $w^{[1]}_j$. And $\large\frac{\partial J}{\partial o}$ is common to *all* the parameters.
###### 12. Page 87
Using `ReLU` (Rectified Linear Unit) as the activation function in the final output layer of a neural network depends on the nature of the problem you are trying to solve. While `ReLU` is a commonly used activation function for hidden layers, it may not always be suitable for the final output layer for the following reasons:
1. **Output Range:** `ReLU` produces output values in the range \[0, ∞). Depending on the problem, you may need your network to produce output values in a different range, such as \[-1, 1] for a regression problem or \[0, 1] for a binary classification problem. `ReLU`'s unbounded positive range makes it unsuitable for constraining output values within specific ranges.
2. **Binary Classification:** In binary classification problems, a common practice is to use a sigmoid activation function in the final output layer. The sigmoid function squashes the output to the range \[0, 1], which can be interpreted as a probability score.
3. **Multiclass Classification:** For multiclass classification problems, the final output layer often uses the `softmax` activation function. `Softmax` ensures that the output values represent class probabilities, and they sum up to 1, which is crucial for assigning an input to one of the multiple classes.
4. **Regression:** In regression tasks where you need to predict continuous values, a linear activation function (i.e., no activation function) is often used in the final output layer. This allows the network to produce real-valued predictions.
5. **Other Customized Needs:** In some cases, you may have specific requirements for the output layer, such as custom activation functions or transformations that are designed to meet the needs of the problem you are addressing.

In summary, the choice of activation function in the final output layer depends on the problem's requirements and the desired output format. `ReLU` is typically used in hidden layers because of its ability to capture complex, non-linear relationships, but for the final output layer, the choice is more problem-specific and may involve different activation functions tailored to the desired output range and interpretation.
###### 11. Page 82-2
In a GLM, the parameters are related to our hypothesis through the link function as:
$$h_\theta(x) = E[T(y)|x;\theta] = g^{-1}(\eta) = g^{-1}(\theta^\intercal \mathbf{x})$$
Note that *all* the parameters of our model are linear (appear to power $1$ and there are no cross-terms), although inside a (potentially) non-linear response function, $g^{-1}$. In this sense, it's a generalized *linear* model. But in a neural network, only the parameters of neurons in any single layer are linear (and inside their activation function): but they are inputted to the next layer and the activation function of that layer causes non-linearity between the parameters of the previous layer with those of the current layer. Consider the example in the book: a neural network shown below
![Pasted image 20231024104342.png](/img/user/Attachments/Pasted%20image%2020231024104342.png)
with the first layer's activations given as
$$\begin{align}
a_1 &= \text{ReLU}(\theta_1x_1+\theta_2x_2+\theta_3) \\
a_2 &= \text{ReLU}(\theta_4x_3+\theta_5) \\
a_3 &= \text{ReLU}(\theta_6x_3+\theta_7x_4+\theta_8) \\
h_\theta(x) &= \theta_9a_1 + \theta_{10}a_2 + \theta_{11}a_3 + \theta_{12} 
\end{align}$$
note that because of terms such as $\theta_9a_1 = \theta_9\text{ReLU}(\theta_1x_1+\theta_2x_2+\theta_3)$ we'll have it either equal to $0$ or to $\theta_9\theta_1x_1+\theta_9\theta_2x_2+\theta_9\theta_3$ which explicitly shows the non-linearity of this neural network in the parameters. This is why neural networks are non-linear models.
>[! ] Addressing a complication
>On page 91, when the author talks about how using a linear activation function essentially
>makes a neural network perform linear regression, he says that the hypothesis becomes:
>$$h_\theta(x) = W^{[2]}a^{[1]} = W^{[2]}z^{[1]} = W^{[2]}W^{[1]}x = \tilde{W}x \tag{1}$$
>with $\tilde{W}$ containing cross terms of the weights from the two layers. Now a question
>arises, can't we redefine $\theta_9\theta_1x_1+\theta_9\theta_2x_2+\theta_9\theta_3 =
>\tilde{\theta}_1x_1+\tilde{\theta}_2x_2+\tilde{\theta}_3x_3$ in the above discussion so that even with a `ReLU` as the activation function we're essentially performing linear regression?
>And the answer to this is that our hypothesis will still be a piecewise function (because `ReLU` is a piecewise function) and piecewise functions are not linear.
>Consider a neural net with two layers (hidden + output) with two neurons in the hidden layer and only one input feature, and `ReLU` as the activation function for the hidden layer. So we have: $$\begin{align}
>a_1 &= \text{ReLU}(\theta_1x_1+\theta_2) \\
>a_2 &= \text{ReLU}(\theta_3x_1+\theta_4) \\
>h_\theta(x) &= \theta_5a_1+\theta_6a_2 + \theta_7 \\
>\Rightarrow h_\theta(x) &= \cases{\theta_6\theta_3x_1 + \theta_6\theta_4 + \theta_7
>\qquad\qquad\qquad\qquad\;\;\;\;\; ; (\theta_1x_1+\theta_2) <0 , (\theta_3x_1+\theta_4)>0\\
>\theta_5\theta_1x_1 + \theta_5\theta_2 + \theta_7 \;\;\;\;\;\qquad\qquad\qquad\qquad ;
>(\theta_1x_1+\theta_2) >0 , (\theta_3x_1+\theta_4) <0\\
>\theta_5\theta_1x_1 + \theta_5\theta_2 + \theta_7 + \theta_6\theta_3x_1 +
>\theta_6\theta_4 + \theta_7 \; ; (\theta_1x_1+\theta_2) >0 , (\theta_3x_1+\theta_4) >0\\
>\theta_7 \qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\;\; ; (\theta_1x_1+\theta_2)
><0 , (\theta_3x_1+\theta_4) <0}
>\end{align}$$
>If we had chosen the identity activation function for this neural net then the hypothesis would've been:
>$$h_\theta(x) = \theta_5\theta_1x_1 + \theta_5\theta_2 + \theta_6\theta_3x_1
>+ \theta_6\theta_4 + \theta_7 = \tilde{\theta}_1x_1+\tilde{\theta}_2$$
>So our hypothesis viewed as a function of $\theta_1\cdots\theta_7$ is not linear in its parameters, while viewed as a function of $\tilde{\theta}_1$ and $\tilde{\theta}_2$ is linear in its parameters. We can learn this hypothesis in two ways:
>1. We can use backpropagation to learn $\theta_1\cdots\theta_7$ and then find $\tilde{\theta}_1$ and $\tilde{\theta}_2$.
>2. Or we can perform a good-old linear regression to directly find $\tilde{\theta}_1$ and $\tilde{\theta}_2$. Note that this will not tell us the values of $\theta_1\cdots\theta_7$.
>
>Either way, we'll get the same hypothesis \[[[Physics/QUESTIONS#<span style="color ff0000">1. Page 91</span>\|1]]]. This is the way in which a neural network with the identity activation function is *equivalent* to linear regression.
>But with the `ReLU` as the activation function, the hypothesis cannot be written as $\tilde{\theta}_1 x + \tilde{\theta}_2$ since it's a piecewise function. That's why it's non linear in its parameters.
>If you're still not convinced then take $\tanh(z)$ as the activation function then we'll get:
>$$h_\theta(x)=\theta_5\tanh(\theta_1x_1+\theta_2) + \theta_6\tanh(\theta_3x_1+\theta_4) + \theta_7$$
>Now it must be clear that there is no reparameterization that can convert this into $h_\theta(x)=\tilde{\theta}_1x_1+\tilde{\theta}_2$.

[[Physics/QUESTIONS#<span style="color ff0000">1. Page 91</span>\|QUESTIONS]]

###### 10. Page 82-1
It is correct to say that neural networks are non-linear models for supervised learning. Neural networks, particularly deep neural networks, introduce non-linearity both in their parameters and in the input data through the activation functions. Activation functions are applied to the linear combinations of inputs and weights at each neuron in the network, which introduces non-linearity in the model.

Some common activation functions used in neural networks include:

1. **Sigmoid Function (Logistic Function):** $f(x) = \frac{1}{1 + e^{-x}}$
2. **Hyperbolic Tangent (Tanh) Function:** $f(x) = \tanh(x) = \frac{e^x - e^{-x}}{e^x + e^{-x}}$
3. **Rectified Linear Unit (`ReLU`):** $f(x) = \max(x, 0)$
4. **Leaky Rectified Linear Unit (Leaky `ReLU`):** $f(x) = \begin{cases}x & \text{if } x > 0\\ ax & \text{otherwise}\end{cases}$, where $a$ is a small positive constant.
These activation functions introduce non-linearities by transforming the weighted sum of inputs, allowing neural networks to model complex, non-linear relationships in the data.

In addition to neural networks, there are many other non-linear models used in machine learning and statistics, including:
1. **Decision Trees:** Decision trees make non-linear decisions by recursively splitting the data based on the values of different features.
2. **Random Forests:** An ensemble of decision trees that can capture complex non-linear relationships in the data.
3. **Support Vector Machines (SVM):** SVMs use non-linear kernel functions to map the data into a higher-dimensional space where a linear decision boundary can be found.
4. **K-Nearest Neighbors (K-NN):** K-NN classifies data points based on the majority class of their nearest neighbors, which can capture non-linear decision boundaries.
5. **Kernel Methods:** Kernel methods, such as the Gaussian Radial Basis Function (RBF) kernel, introduce non-linearity in various machine learning algorithms.
6. **Polynomial Regression:** In polynomial regression, the relationship between the input features and the output is modeled as a polynomial equation, introducing non-linearity.
7. **Gaussian Processes:** Gaussian processes are a non-linear, non-parametric model used for regression and classification tasks.

These are just a few examples of non-linear models in machine learning and statistics. The choice of model depends on the specific problem and the nature of the data you are working with.
###### 9. Page 37
Summing over $y$ on both sides gives:
$$\begin{align} \sum\limits_{y}{p(y|x)} &= \sum\limits_{y}{\frac{p(x|y)p(y)}{p(x)}}\\
1 &= \frac{1}{p(x)}\sum\limits_{y}{p(x|y)p(y)}\\
p(x) &= p(x|y=1)p(y=1)+p(x|y=0)p(y=0) \end{align} $$
###### 8. Page 36
Logistic regression gives the probability of $y=1$ and hence of $y=0$ then if $P(y=1)>0.5$ then it our prediction is that $y=1$. So this line, aka the decision boundary, is this $0.5$ horizontal line.
###### 7. Page 33
We can write $a(\eta)=-\log(\phi_k) \times (\eta^T\eta)^0$ to explicitly show it as a function of $\eta$.
###### 6. Page 33
The link function is defined as $\eta=g(\text{E}[T(y)])$. And $\text{E}[T(y)]$ is
$$\large\begin{align}
\text{E}[T(y)] &= \sum\limits_{i=1}^k \phi_iT(i)\\
&= \phi_1\begin{pmatrix} 1 \\ \vdots \\ 0 \end{pmatrix}+\cdots+\phi_{k-1}\begin{pmatrix} 0 \\ \vdots \\ 1 \end{pmatrix} + \phi_k\begin{pmatrix} 0 \\ \vdots \\ 0 \end{pmatrix}\\
&= \begin{pmatrix} \phi_1 \\ \vdots \\ \phi_{k-1} \end{pmatrix}
\end{align}$$
So the link function is defined as $g:\mathbb{R}^{k-1}\rightarrow\mathbb{R}^{k-1}$ such that for a given $(k-1)\times1$ column vector, $\large\vec{\phi}$, its output is also a $(k-1)\times1$ column vector, $\large\vec{\eta}$, whose $i^th$ component is $\large\eta_i=\log \frac{\phi_i}{\phi_k}$ where $\phi_k=1-\sum\limits_{i=1}^{k-1}\phi_i$.
###### 5. Page 33
The identity $1\{y=k\}=1-\sum\limits_{i=1}^{k-1}1\{y=i\}$ can be understood as follows: when $y=k$ the left side is $1$ and on the right side each term of the sum is $0$ so the right side is also $1$, and when $y\ne k$ (some other value from $\{1,2,\dotso,k-1\}$) then the left side is $0$ and only one term in the sum on the right is $1$ and all the other terms are $0$ so the right side becomes $1-1=0$.
###### 4. Page 32
We have defined $T:S\rightarrow\mathbb{R}^{k-1}$ where $S=\{1,2,\dotso,k\}$. Since $y$ is a random variable, $T(y)$ is also a random variable (depending on the value of $y$ it will be a column vector $T(y$)) and its $i^{th}$ component, $(T(y))_i$, is also a random variable (it'll either be $0$ or $1$). So we *can* talk about its expectation value, $E[(T(y))_i]$. Now, $(T(y))_i$ is just a binary random variable with probability $\phi_i$ of being $1$ which is when $y=i$.

###### 3. Page 31
And ordinary least squares also has $h_{\theta}(x)=\theta
{ #T}
 x$. Note that the determination of the $\boldsymbol{\theta}$ is a different issue. We can show that the ordinary least squares and the logistic regression are special cases of GLMs by showing that for an appropriate choice of $p(y|x)$ and under the three assumptions we've made for a GLM we get $h_{\theta}(x)$ equal to the expressions of ordinary least squares and the logistic regression.
###### 2. Page 27
$$\begin{align} p(y;\eta) &= b(y)\exp(\eta^TT(y)-a(\eta))\\ &= \frac{b(y)\exp(\eta^TT(y))}{\exp(a(\eta))} \end{align}$$
Now we can clearly see that the quantity $e^{-a(\eta)}$ is a normalizing factor w.r.t. $y$ since it doesn't depend on it.
###### 1. Page 16
Note that $(A^TB)^T=B^T(A^T)^T=B^TA$, so if we are constraining $A^TB=B^TA$, that implies $(A^TB)^T=A^TB$, meaning $A^TB$ is symmetric: but if $A$ and $B$ are vectors then $A^TB$ is definitely symmetric since it's a scalar.

$\large{y^{(i)}=\boldsymbol{\theta}^T\mathbf{x}^{(i)}+\epsilon^{(i)}}$ 

###### item - page 99
First of all, $q_{ab}n^a=N_a n^a=0$ means $q_{ab}\; n^a=0$ and $N_a n^a=0$, and not that $q_{ab}\;n^a=N_a n^a$. Now, $N_a n^a = q_{ab}N^b n^a$ which is the inner product of two perpendicular vectors hence it's $0$.

## Quantum Measurement Theory
### QMT and its Applications - Kurt Jacobs
###### 1. Page 20
This table is meant to give $P(y|x)$ so it should be read vertically: when $x=0$ we get $y=0$ with probability $\alpha$ and $y=1$ with probability $1-\alpha$ and when $x=1$ we get $y=0$ with probability $\beta$ and $y=1$ with probability $1-\beta$ where $\alpha$ and $\beta$ are not necessarily equal or related. Why are we assuming $\beta=1-\alpha$?
P.ANS. = Since we know from Bayes' theorem that $P(y|x)$ is related to $P(x|y)$:
$$P(x|y)=\frac{P(y|x)P(x)}{P(y)} \;\;\;\xleftrightarrow{\text{\;\;\;\;}}\;\;\; P(y|x)=\frac{P(x|y)P(y)}{P(x)}$$Interchanging the $x$ and $y$ symbols in either of them yields the other so this symmetry requires that $P(x|y)$ must have the same distribution as $P(y|x)$: when $x=0$ the probabilities of $y$ to be $0$ or $1$ are $\alpha$ and $1-\alpha$ respectively, similarly, when $y=0$ the probabilities of $x$ to be $0$ or $1$ are $\alpha$ and $1-\alpha$ respectively too. This is corroborated by the line below equation 1.7 where it's using this table to find values of $P(\textbf{0}|1)$ and $P(\textbf{1}|1)$.


## Quantum Gravity
### 1. Mustafa Saeed[ ](<D:\Knowledge\BOOKS\Physics\Advance Physics\QG\Cosmological Perturbation Theory in a Matter-Time Gauge - Mustafa Saeed.pdf>)
###### 1. Page 114
Note that for preservation under time-evolution we usually require the time-derivative of a quantity to be zero so that it remains the same as time progresses; but when that quantity is itself time (like in the dust-time gauge, $\phi=t$) then we should have its time-derivative to be $1$ for it to be preserved with time since then $d\phi=dt$.
###### 2. Page 82
The first possibility is when $\dot{\phi}_m$ turns out to be a linear combination of the primary constraints: $\dot{\phi}_m = \beta_n\phi_n$ and pulling the $\phi_m$ term out to show it explicitly we get $\dot{\phi}_m = \alpha\phi_m + \beta_n\phi_n$.
###### 3. 




# QUESTIONS
## General Relativity
### 1. Schutz 2e[ ](<D:\Knowledge\BOOKS\Physics\Advanced Physics\General Relativity\A First Course in General Relativity 2e - Schutz.pdf>)
###### <font color="#ff0000">30. Chapter 3, Page </font>

###### <font color="#ff0000">29. Chapter 3, Page </font>

###### <font color="#ff0000">28. Chapter 3, Page </font>

###### <font color="#ff0000">27. Chapter 3, Page </font>

###### <font color="#ff0000">26. Chapter 3, Page </font>

###### <font color="#ff0000">25. Chapter 3, Page </font>

###### <font color="#ff0000">24. Chapter 3, Page </font>

###### <font color="#ff0000">23. Chapter 3, Page </font>

###### <font color="#ff0000">22. Chapter 3, Page </font>

###### <font color="#ff0000">21. Chapter 3, Page </font>

###### <font color="#ff0000">20. Chapter 3, Page </font>

###### <font color="#ff0000">19. Chapter 3, Page </font>

###### <font color="#ff0000">18. Chapter 3, Page </font>

###### <font color="#ff0000">17. Chapter 3, Page </font>

###### <font color="#ff0000">16. Chapter 3, Page </font>

###### <font color="#ff0000">15. Chapter 3, Page </font>

###### <font color="#ff0000">14. Chapter 3, Page </font>

###### <font color="#ff0000">13. Chapter 3, Page </font>

###### <font color="#ff0000">12. Chapter 3, Page </font>

###### <font color="#ff0000">11. Chapter 3, Page 74</font>
**Q** = I forgot/don't understand how/why the metric is used to perform raising/lowering of indices: why can't we use some other $\binom{0}{2}$ symmetric tensor to do this? 
**P.ANS.** = 
###### <font color="#ff0000">10. Chapter 3, Page 68</font>
**Q** = Can the metric map vectors into one-forms and one-forms into vectors?
**P.ANS.** = Yes, see subsection of 3.5 titled, "The inverse: going from $\large\tilde{A}$ to $\large\vec{A}$".
###### <font color="#ff0000">9. Chapter 3, Page 64</font>
**Q** = I cannot make complete sense of the two bracketed paragraphs.
**P.ANS.** = 
###### <font color="#ff0000">8. Chapter 2, Page 44, 45</font>
**Q** = The scalar product defined as $\vec{A}\cdot \vec{B} = -A^0B^0+A^1B^1+A^2B^2+A^3B^3$ doesn't uphold one of the properties of an inner product which says that $d(v,v)\ge0 \;\;\text{and}\;\; d(v,v)=0 \;\;\text{iff}\;\; v=0$ since now it can be negative and zero for non-zero vectors. Just to be clear, this means that it's not an inner product, right?
**P.ANS.** = Yes.
###### <font style="color:rgb(255,0,0);">7. Chapter 2, Page 44</font>
**Q** = I don't know/haven't seen the proof of the fact that the interval is invariant under the Lorentz transformation.
**P.ANS.** = Read chapter 1 😃
###### <font style="color:rgb(255,0,0);">6. Chapter 2, Page 43</font>
**Q** = Although I *think* I understand the point this paragraph is trying to make, but I cannot understand its importance: the law of conservation of 4-momentum is about a *single* collision while this paragraph discusses multiple collisions. Since the law holds for each collision separately then we can simply associate a single momentum vector with each collision: the net momentum before the collision gives us one vector for before the collision, and the net momentum after the collision gives us another vector for after the collision, but from the conservation law these two are the same vector.
**P.ANS.** = I think the author is making a fuss out of this 😜
###### <font style="color:rgb(255,0,0);">5. Chapter 2, Page 34</font>
**Q** = What about something like $T^{\gamma}E_{\alpha \gamma}$: does Einstein's summation convention make sense for this so that it's $\sum\limits_{\gamma=0}^3 T^{\gamma}E_{\alpha \gamma}$?
**P.ANS.** = 
###### <font style="color:rgb(255,0,0);">4. Chapter 2, Page 34</font>
**Q** = Why/How come the Lorentz transformation is used to find components in new/old basis?
**P.ANS.** = Read chapter 1 :)
###### <font style="color:rgb(255,0,0);">3. Chapter 1, Page 8</font>
**Q** = I cannot show that the angles made by the $\bar{t}$-axis with the $t$-axis and the angle made by the $\bar{x}$-axis with the $x$-axis are equal.
**ANS** = 
###### <font style="color:rgb(255,0,0);">2. Chapter 1, Page 3</font>
**Q** = The geometrical definition of an inertial frame is given and said that only an unaccelerated frame can keep its clocks synchronized. I have a few concerns about the required properties:
1. I cannot think of any frame in which the distance between P1 and P2 is a function of time. And, isn't this included in the third property requiring the geometry to be Euclidean?
2. What does it really mean to say that the geometry is Euclidean? Does it mean a flat space with the Euclidean metric? If so, then the first property is indeed included in this since the Euclidean metric is independent of time.
3. I have to come back to this definition to see how only an unaccelerated frame can keep its clocks synchronized.
###### <font style="color:rgb(255,0,0);">1. Chapter 1, Page 3</font>
**Q** = The footnote reads, "It is easy to see that gravitational fields cause problems for SR. If an astronaut in orbit about Earth holds a bowl of soup, does the soup climb up the side of the bowl in response to the gravitational ‘force’ that holds the spacecraft in orbit? Two astronauts in different orbits accelerate relative to one another, but neither feels an acceleration. Problems like this make gravity special, and we will have to wait until Ch. 5 to resolve them. Until then, the word ‘force’ will refer to a nongravitational force." However, I cannot understand how these are problems for SR and how these scenarios are specific to the gravitational force only.
The answer to the first question is, I think, that the soup will not rise on any side of the bowl since the soup, the bowl, and the astronaut are all in free fall due to a centripetal force (gravity in this case). But any other centripetal force will also cause this same behavior. The second scenario is (I think) more understandable: the astronauts don't feel any acceleration and they might (wrongfully) conclude themselves to be in inertial frames and hence the predictions of SR will not hold in these 'inertial' frames.
### 2. Carroll[ ](<D:\Knowledge\BOOKS\Physics\Advanced Physics\General Relativity\Spacetime and Geometry - Sean Carroll.pdf>)
###### <font color="#ff0000">1. Chapter 2, Page 59</font>
**Q** = The domain of the map $\phi_\alpha\circ \phi_\beta^{-1}$ is $\phi_\beta(U_\alpha\cap U_\beta)$ and its range/image is $\phi_\alpha\circ \phi_\beta^{-1}\left(\phi_\beta(U_\alpha\cap U_\beta)\right) = \phi_\alpha\left(\phi_\beta^{-1}\left(\phi_\beta(U_\alpha\cap U_\beta)\right)\right)=\phi_\alpha(U_\alpha\cap U_\beta)$ and hence just like any other map it's onto its image. Then why are we explicitly saying this as if it's a requirement/additional constraint we're putting on this map? I think the only constraint is the $C^{\infty}$ requirement.

## Computational Physics
### 1. Andrew Ng Notes[ ](<D:\Knowledge\BOOKS\Physics\Computational Physics\Machine Learning\Andrew Ng Notes.pdf>)
###### <span style="color:red">1. Page 91</span>
**Q** = How is a neural network with the identity activation function equivalent to linear regression? Take the example of a two-layer network with $2$ neurons in the hidden layer, $1$ neuron in the output layer, and only $1$ feature. Take the activation functions to be identity:
$$\begin{align}
a_1 &= \theta_1x+\theta_2\\
a_2 &= \theta_3x+\theta_4\\
h_\theta(x) &= \theta_5a_1+\theta_6a_2+\theta_7\\
&= (\theta_5\theta_1+\theta_6\theta_3)x+(\theta_5\theta_2+\theta_6\theta_4+\theta_7) \tag{1}\\
&= \tilde{\theta}_1x + \tilde{\theta}_2 \tag{2}
\end{align}$$
- Viewed as a function of $\theta_1,\cdots,\theta_7$, the hypothesis is non-linear in its parameters.
- Viewed as a function of $\tilde{\theta}_1,\tilde{\theta}_2$, the hypothesis is linear in its parameters.
We can learn $(1)$ using backpropagation getting the values of the parameters that minimize the cost function, $\theta_1^*,\cdots,\theta_7^*$. And we can learn $(2)$ using linear regression to find $\tilde{\theta}_1^*$ and $\tilde{\theta}_2^*$. Now, it intuitively makes perfect sense that since our hypothesis is the same, and our cost function is the same, and our learning algorithm is the same, then we should get those values of these stared-parameters such that:
$$\begin{align}\tilde{\theta}_1^* &= \theta_5^*\theta_1^* + \theta_6^*\theta_3^* \tag{3}\\
\tilde{\theta}_2^* &= \theta_5^*\theta_2^* + \theta_6^*\theta_4^* + \theta_7^* \tag{4}\\
\end{align}$$
That is, the values of the parameters, $\theta_1,\cdots,\theta_7$, that minimize the cost function with $h_\theta(x)$ should combine according to $(3)$ and $(4)$ to give us the values of $\tilde{\theta}_1$ and $\tilde{\theta}_2$ that minimize the cost function with $h_{\tilde{\theta}}(x)$. However, I cannot show this mathematically.


## Quantum Gravity
### 1. Mustafa Saeed[ ](<D:\Knowledge\BOOKS\Physics\Advance Physics\QG\Cosmological Perturbation Theory in a Matter-Time Gauge - Mustafa Saeed.pdf>)
###### <span style="color: red">1. Page 108</span>
**Question** = Is this correct: the spatial metric, $q_{ab}$, has $6$ independent components (hence $6$ degrees of freedom), similarly, $\pi_{ab}$ also has $6$ independent components hence totaling $12$ degrees of freedom. The Hamiltonian $H^{GR}$ is a scalar so it represents a single first-class constraint, while $C_a^{GR}$ is a spatial vector therefore it represents $3$ first-class constraints totaling $4$ first-class constraints. 

###### <span style="color:#ff0000">2. Page 80</span>
**Question** = I wonder how the existence of relations between the phase space variables prevents the existence of an invertible map between the velocities and the conjugate momenta. $$p_i = \frac{\partial L}{\partial \dot{q}_i}$$
**Answer** = 
###### <span style="color:#ff0000">3. Page 84</span>
**Question** = It's said that in order to avoid the $\dot{\phi}_m=\lambda$ case we specify the Lagrangian such that we do not encounter this case.
1. How do we know that rewriting the Lagrangian avoids this case?
2. Why can we do this without affecting anything physical in the theory (i.e., the dynamics of the system)?
3. How do we do this rewriting?
**Answer** = 
###### <font color="#ff0000">4. Page </font>
**Question** = 
**Answer** = 

> [!PDF|yellow] [[Cosmological Perturbation Theory in a Matter-Time Gauge - Mustafa Saeed.pdf#page=84&selection=28,15,29,25&color=yellow|p.84]]
> We specify the Lagrangian such that we do not encounter this condition.

> [!PDF|yellow] [[Cosmological Perturbation Theory in a Matter-Time Gauge - Mustafa Saeed.pdf#page=84&selection=28,15,29,25&color=yellow|p.84]]
> We specify the Lagrangian such that we do not encounter this condition.


---
# INSIGHTS 
## General Relativity
### 1. Schutz 2e[ ](<D:\Knowledge\BOOKS\Physics\Advanced Physics\General Relativity\A First Course in General Relativity 2e - Schutz.pdf>)
###### 1. This insight is from another notes.
![Pasted image 20240129113741.png](/img/user/Attachments/Pasted%20image%2020240129113741.png)
This is a way to create an infinite force.


###### 2. Hz vs $s^{-1}$
![Pasted image 20240424102356.png](/img/user/Attachments/Pasted%20image%2020240424102356.png)
From Kurt Jacobs book on "QMT and its Applications"


---
# IDEAS
These are ideas I get from different sources for further exploration.
## Random Sources
###### 4. Earth is a rogue planet
In [this](https://youtu.be/tZ2o2IwS54Q?list=PLnaXrumrax3Wyn1oMYWYlpcwrc76Nm40Q&t=607) video, Neil deGrasse Tyson says that if you read Genesis literally it says that the earth was created before the sun; a possible explanation for this could be that the earth was part of another solar/star system and once its star went supernova the earth became a rogue planet and then our current sun was born and it caught the wandering earth into its gravitational bound.
## General Relativity
###### 1. Series solution of Geodesic equation for SC metric
For the Schwarzschild metric we write down the geodesic equations which turn out to be coupled PDEs hence we abandon solving them: we instead take the route of extremizing the Lagrangian which gives us the geodesics. I was wondering, what if we attempt a power series expansion of the four coordinates in order to convert the coupled PDEs into coupled algebraic equations? Since the geodesics are smooth this expansion is allowed.

###### 2. Photon Sphere vs $\Lambda$
the photon sphere remains at 3M even with the cosmological constant taken into account. What's the physical reason for this? Does dark energy not affect energy (i.e., photons)?

## Mathematical Physics
###### 1. Solving D.Es.
In the book, "A visual introduction to differential forms and calculus on manifolds" on page 457 in Appendix B there is this line, "By increasing the number of variables we turned a second-order differential equation into a system of first-order differential equations. This makes solving the differential equations easier, but at the cost of having to solve for more variables."
Maybe this can be used in some way to reduce the complexity of a D.E..

###### 2. Gauge Freedom in DEs.
Every differential equation (possibly) has a gauge freedom: so the theory/system the equation represents has this gauge freedom.


---
# Anki Cards
## General Relativity
### 1. Schutz 2e[ ](<D:\Knowledge\BOOKS\Physics\Advanced Physics\General Relativity\A First Course in General Relativity 2e - Schutz.pdf>)
###### 1. Page 48
Make an Anki card about the proof of 2.34
###### 2. Page 61
Why do we focus/care about a change of basis? (check my comment)

---
[[Cosmological Perturbation Theory in a Matter-Time Gauge - Mustafa Saeed.pdf#page=86&annotation=1696R|p.86]]
![SmartSelect_20240911_114943_touchnotes.jpg](/img/user/Attachments/SmartSelect_20240911_114943_touchnotes.jpg)

---


> ([[Cosmological Perturbation Theory in a Matter-Time Gauge - Mustafa Saeed.pdf#page=86&annotation=1707R|Cosmological Perturbation Theory in a Matter-Time Gauge - Mustafa Saeed, p.86]])
> correspond to the same physical state

---

---
[[Cosmological Perturbation Theory in a Matter-Time Gauge - Mustafa Saeed.pdf#page=86&annotation=1707R|Cosmological Perturbation Theory in a Matter-Time Gauge - Mustafa Saeed, p.86]]

---
[[Cosmological Perturbation Theory in a Matter-Time Gauge - Mustafa Saeed.pdf#page=86&annotation=1707R|correspond to the same physical state]]
[[Cosmological Perturbation Theory in a Matter-Time Gauge - Mustafa Saeed.pdf#page=86&annotation=1707R|Cosmological Perturbation Theory in a Matter-Time Gauge - Mustafa Saeed, p.86]]

---
> [!PDF|0, 255, 0] [[Cosmological Perturbation Theory in a Matter-Time Gauge - Mustafa Saeed.pdf#page=86&annotation=1707R|Cosmological Perturbation Theory in a Matter-Time Gauge - Mustafa Saeed, p.86]]
> correspond to the same physical state

> [!PDF|255, 0, 0] [[Cosmological Perturbation Theory in a Matter-Time Gauge - Mustafa Saeed.pdf#page=86&annotation=1707R|Cosmological Perturbation Theory in a Matter-Time Gauge - Mustafa Saeed, p.86]]
> correspond to the same physical state

[[Cosmological Perturbation Theory in a Matter-Time Gauge - Mustafa Saeed.pdf#page=86&annotation=1707R|Cosmological Perturbation Theory in a Matter-Time Gauge - Mustafa Saeed, p.86]]

> [!PDF|255, 0, 0] [[Cosmological Perturbation Theory in a Matter-Time Gauge - Mustafa Saeed.pdf#page=86&annotation=1707R|Cosmological Perturbation Theory in a Matter-Time Gauge - Mustafa Saeed, p.86]]
> > correspond to the same physical state
> 
> this is some text.

