## 2.1 BASIC CONCEPTS

In many probabilistic models, the outcomes are of a numerical nature, e.g., if they correspond to instrument readings or stock prices. In other experiments, the outcomes are not numerical, but they may be associated with some numerical values of interest. For example, if the experiment is the selection of students from a given population, we may wish to consider their grade point average. When dealing with such numerical values, it is often useful to assign probabilities to them. This is done through the notion of a __random variable__.

Given an experiment and the corresponding set of possible outcomes (the sample space), a random variable associates a particular number with each outcome. We refer to this number as the __numerical value__ or the __experimental value__ of the random variable. __Mathematically, a random vari- able is a real-valued function of the experimental outcome.__

There are several basic concepts associated with random variables, which are summarized below.

##### Main Concepts Related to Random Variables

* A __random variable__ is a real-valued function of the outcome of the experiment.
* A __function of a random variable__ defines another random variable.
* We can associate with each random variable certain “averages” of interest, such the __mean__ and the __variance__.
* A random variable can be conditioned on an event or on another random variable.
* There is a notion of independence of a random variable from an event or from another random variable.

A random variable is called __discrete__ if its range (the set of values that it can take) is finite or at most __countably infinite__. 

__A random variable that can take an uncountably infinite number of values is not discrete.__

##### Concepts Related to Discrete Random Variables

Starting with a probabilistic model of an experiment:

* A discrete random variable is a real-valued function of the outcome of the experiment that can take a finite or countably infinite number of values.
* A (discrete) random variable has an associated __probability mass function (PMF)__, which gives the probability of each numerical value that the random variable can take.
* A function of a random variable defines another random variable, whose PMF can be obtained from the PMF of the original random variable.

## 2.2 PROBABILITY MASS FUNCTIONS



