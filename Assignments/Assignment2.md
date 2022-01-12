<!-- 
<p align="center">
<img width = 500 height = 400 src="../assets/assignment2_start.jpeg"/></br>
<i>Glad to see you all</i>
</p> -->

<h1 align="center">Assignment 2</h1>

<p align="center">

You all have gone through the below listed things in the second workshop : 
 
- Linear Regression
- Logistic Regression
- Gradient Descent(Optimization)
</p>

**Firstly Let's progress our Trip :train: of Regression and Optimization from Workshop**

## Linear Regression

We are adding a few definitions to clarify some basic concepts before progressing with the Assignment.

**Data Distribution**

It is quite clear that Regression assumes a linear variation of data. For Ex-
<p align="center">
<img width = 500 height = 200 src="../assets/compare.png"/></br>
</p>
In Fig-(a) displays a good fit with linear Regression as the data distribution is almost linear, on the other hand in Fig-(b) showing a non linear data distribution, linear regression cannot perform well. These non linear data requires fitting complex models which you will learn later.</br>
</br>

**Equation**

Although Regression is applicable for any number of dimensions, here we are writing it for 2D space which involves finding two optimal parameters
<p align="center">
<img width = 500 height = 300 src="../assets/linear_eqn.jpg"/></br>
</p>

Here `m` and `b` are the two parameters which need to be determined for finding the optimal line for given data.

**Loss and Update Eqn**

Most important is to calculate loss( **Mean Squared Error(MSE)** in case of Regression) and update the equation for Gradient descent.

<p align="center">
<img width = 300 height = 200 src="../assets/loss_lin.png"/>
<img width = 300 height = 200 src="../assets/update_lin.png"/></br>
Mean Squared error Loss(Left) and Update equation(Right) 
</p>

**Implementation**

[Resource for implementing Linear Regression from scratch](https://towardsdatascience.com/coding-linear-regression-from-scratch-c42ec079902) 


<h1 align="center">Your Task</h1>

In this Assignment you will be solving a trivial fitting problem on a famous(one of the most important equation in math) non linear data distribution known as Gaussian(Normal) Distribution which can be graphically depicted as

<p align="center">
<img width = 300 height = 200 src="../assets/gaussian.jpg"/>
<img width = 300 height = 200 src="../assets/gaussian_noisy.png"/></br>
Ideal Curve(Left) and Noisy Real Data(Right) 
</p>

In real world dataset the data is not ideal as it contain erroneous enteries accumulated from different sources but we can approximate any normal data to it's nearest optimal normal curve like shown below.

<p align="center">
<img width = 500 height = 300 src="../assets/gaussian_fit.png"/> 
</p>

So those who aren't knowledgable about Gaussian(Normal) Distribution, below are the resources that we followed.  Kindly go through them one by one. 

### Importance of Normal distribution
* [What is Normal Distribution and why it is important](https://medium.com/analytics-vidhya/the-normal-distribution-for-data-scientists-6de041a01cb9#:~:text=The%20normal%20distribution%20is%20a,in%20the%20data%20science%20curriculum.)
* [Blog 2](https://towardsdatascience.com/the-powers-of-normal-distribution-4cbb06e4a955)
* [Why Data scienctists love Gaussian](https://towardsdatascience.com/why-data-scientists-love-gaussian-6e7a7b726859)

So, If you went through above links you will encounter an equation something like

<p align="center">
<img width = 400 height = 300 src="../assets/formula_normal.png"/></br>
it contains two parameters **mu** and **sigma**
</p>

Hence, just like the equation of line `y=mx+b` which contains two parameters `m` and `b`, here are two parameters `mu` and `sigma`. Your task is find these two optimal parameters for the given noisy data. 

How To Start:-

- Create a copy of this [**JUPYTER NOTEBOOK**](https://colab.research.google.com/drive/1EoRNvI1FDWaoaiipwEpp8uWhxV3Nqs_G?usp=sharing).
- Run the first cell which will tell you the optimal `mu` and `sigma` for the data. These values help you later to verify your code is correct or not.
- Now take intutition from above implemetation of linear regression.
- Use Same MSE (Mean Squared) loss.
- Calculate Loss derivative w.r.t `mu` and `sigma` to find updated equation to perform gradient descent.
- Run Gradient Descent Until Optimization.(And as a sanity check, ensure that the parameter values you get after convergence is close to the optimal ones from first cell.)


### To Submit-

Create a Zip Consisting
 - image of output from first cell
 - Loss/Cost Curve (Take reference from above linear regression implementation).
 - Notebok Containing your final code. In the last cell of notebook, comment the number of iterations your code took for convergence, the learning rate you used and the `mu` and `sigma` your code output.

**Deadline will be informed later, just work patiently and enjoy this task, we will provide enough time so don't worry about time.** 


