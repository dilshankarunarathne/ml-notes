# Machine Learning 

<pre>
Machine Learning, is the field of study that gives computers the ability 
to learn without being explicitly programmed. 
                                                  - Arthur Samuel (1959)
</pre>

<pre>
Well-posed Learning Problem: A computer program is said to learn from 
experience E, with respect to some task T, and some performance 
measure P - if its performance on T, as measured by P, improves with experience E.
                                                  - Tom Mitchell (1959)
</pre>

## Types of Machine learning algorithms 

+ Common:
  + Supervised learning 
  + Unsupervised learning
+ Other:
    + Reinforcement learning
    + Recommender systems

### Supervised learning

![Plot of prices against the size of houses](\assets\1-housing-price.png "assets/1-housing-price")

With this given data set, we can use a liner, quadratic or any other 
algorithm to presume the value of a certain house based on it's size.   
This is a good example of **supervised learning**. We give the algorithm 
a set of "**right answers**" for it to learn.  
After we gave the algorithm a dataset of **right prices** those houses were
sold, what the algorithm had to do was, to generate more of these prices.
This is also called a **Regression** problem. We are trying to predict 
**a continuous valued output**. 

Consider another scenario. We have given a dataset of people who tested 
for brest cancer against the type of the brest cancer detected. Let's say 
0 - no cancer, 1 - type A, 2 - type B, 3 - type 3 (this is not a real thing...)  
In this case, we have to predict which event happens in a set of possible 
events. This is an example of a **Classification problem**.  

### Unsupervised learning

Here's a dataset, find some structure in it. 