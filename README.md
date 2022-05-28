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
![Clustered plot](\assets\2-clusters.png "assets/2-clusters")  
Given this dataset, the algorithm should find that the data is divided
into two clusters.  

(Mostly) in unsupervised learning, what the dataset actually mean doesn't 
matter to the algorithm.  
They try to identify structures in the data.  
This is also called 'clustered learning'.  

#### The Cocktail Party Problem 

Consider this scenario...   
At a cocktail party, there are two (main) people talking in two different 
groups. (Lets isolate these two speakers, and forget about all the other 
listeners in there)...   
If we put two microphones, one closer to Speaker #1, and the other closer 
to Speaker #2.  

![Cocktail Party](\assets\3-cocktail-party.png "assets/3-cocktail-party")

When we listen to those two recordings, both of those would contain - both 
Speaker #1 and Speaker #2 's voice.  
When (one of or both of) these recordings are given to an unsupervised 
learning algorithm, that algorithm should be able to identify that there 
are two different sources of data, that are mixed together into the same 
dataset. And it should be able to isolate each source and give two outputs.  

So, anyone might see this example of unsupervised learning and think, 
this algorithm must be very complicated to implement. And it must be 
very hard to build an application like this...  

The algorithm sure is not easy to implement. But thankfully, with the 
correct programming environment, there are libraries that we can use. 
And actually, we can build this kind of application with just one line of 
code...  

![A single line of code](\assets\4-one-line.png "assets/4-one-line")

In this, we will be using [Octave](https://www.gnu.org/software/octave).  
[Octave](https://www.gnu.org/software/octave) is an open-source software. 
With an application like [Octave](https://www.gnu.org/software/octave) 
or [Matlab](https://www.mathworks.com/products/matlab.html), we can 
implement algorithms like these with only a few lines of code. Also, with
[Octave](https://www.gnu.org/software/octave) environment, we can prototype 
our algorithms before we build applications or implement them with a 
language like C++ or Java.  

## Model Representation

![Notations](C:\Projects\studying-ml\assets\5-notation.png "assets\5-notation.png")

**m** = Number of training examples  
**x** = An **input** variable / features  
**y** = An **output** variable / target variable  
**(x,y)** = One training example  
**(x<sup>i</sup>,y<sup>i</sup>)** = i<sup>th</sup> training example  
**h** = hypothesis  

![The Model](C:\Projects\studying-ml\assets\6-model.png "assets\6-model.png")

Hypothesis **h** is a function that maps from input x's to y's.  

The term _hypothesis_ is not actually a great name in this sense. But it 
was used since the early days of machine learning 