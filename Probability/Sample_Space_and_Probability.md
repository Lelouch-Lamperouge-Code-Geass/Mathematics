## 1.1 SETS

A __set__ is a collection of objects, which are the elements of the set. If S is a set and x is an element of S,we write ```x ∈ S```. If x is not an element of S,we write ```x ∈/ S```. A set can have no elements, in which case it is called the empty set, denoted by Ø.

If S contains infinitely many elements x1, x2, . . ., which can be enumerated in a list (so that there are as many elements as there are positive integers) we write ```S = {x1,x2,...}```, and we say that S is __countably infinite__. For example, the set of even integers can be written as {0, 2, −2, 4, −4, . . .}, and is countably infinite.

Alternatively, we can consider the set of all x that have a certain property P, and denote it by ```{x|x satisfies P}```. (The symbol “|” is to be read as “such that.”) For example the set of even integers can be written as {k | k/2 is integer}. Similarly, the set of all scalars x in the interval [0, 1] can be written as {x | 0 ≤ x ≤ 1}. Note that the elements x of the latter set take a continuous range of values, and __cannot be written down in a list__ (a proof is sketched in the theoretical problems); such a set is said to be __uncountable__.

If every element of a set S is also an element of a set T, we say that S isasubsetofT,andwewriteS⊂TorT⊃S. IfS⊂TandT⊂S,the two sets are equal, and we write S = T. It is also expedient to introduce a universal set, denoted by Ω, which contains all objects that could conceivably be of interest in a particular context. Having specified the context in terms of a universal set Ω, we only consider sets S that are subsets of Ω.

##### Set Operations

The __complement__ of a set S, with respect to the universe Ω, is the set {x ∈ Ω|x ∈/ S} of all elements of Ω that do not belong to S, and is denoted by Sc. Note that Ωc = Ø. 

The __union__ of two sets S and T is the set of all elements that belong to S or T (or both), and is denoted by S ∪ T . The intersection of two sets S and T is the set of all elements that belong to both S and T, and is denoted by S∩T. Thus,

```
S ∪ T = {x | x ∈ S or x ∈ T }, 
S ∩ T = {x | x ∈ S and x ∈ T }.
```

Two sets are said to be __disjoint__ if their intersection is empty. More generally, several sets are said to be disjoint if no two of them have a common element. A collection of sets is said to be a partition of a set S if the sets in the collection are disjoint and their union is S.

If x and y are two objects, we use (x,y) to denote the ordered pair of x and y. The set of scalars (real numbers) is denoted by R; the set of pairs (or triplets) of scalars, i.e., the two-dimensional plane (or three-dimensional space, respectively) is denoted by R2 (or R3, respectively).

##### The Algebra of Sets

Set operations have several properties, which are elementary consequences of the definitions. Some examples are:

```
S∪T =T∪S,
S ∩(T ∪U) = (S ∩T)∪(S ∩U),
(Sc)c =S, S ∪ Ω = Ω,
S∪(T∪U)=(S∪T)∪U,
S ∪(T ∩U) = (S ∪T)∩(S ∪U),
S∩Sc =Ø, S ∩ Ω = S.
```

## 1.2 PROBABILISTIC MODELS

##### Sample Spaces and Events

![alt](http://slideplayer.com/slide/6415849/22/images/9/Probabilistic+models+Sample+space:+set+of+all+possible+outcomes+of+an+experiment+(mutually+exclusive,+collectively+exhaustive).jpg)

Every probabilistic model involves an underlying process, called the __experiment__, that will produce exactly one out of several possible __outcomes++. The set of all possible outcomes is called the __sample space__ of the experiment, and is denoted by Ω. A subset of the sample space, that is, a collection of possible outcomes, is called an __event__. There is no restriction on what constitutes an experiment. For example, it could be a single toss of a coin, or three tosses, or an infinite sequence of tosses. However, it is important to note that in our formulation of a probabilistic model, there is only one experiment. So, three tosses of a coin constitute a single experiment, rather than three experiments.

The sample space of an experiment may consist of a finite or an infinite number of possible outcomes. Finite sample spaces are conceptually and math- ematically simpler. Still, sample spaces with an infinite number of elements are quite common. For an example, consider throwing a dart on a square target and viewing the point of impact as the outcome.

##### Choosing an Appropriate Sample Space


Regardless of their number, different elements of the sample space should be distinct and __mutually exclusive__ so that when the experiment is carried out, there is a unique outcome. For example, the sample space associated with the roll of a die cannot contain “1 or 3” as a possible outcome and also “1 or 4” as another possible outcome. When the roll is a 1, the outcome of the experiment would not be unique.

A given physical situation may be modeled in several different ways, de- pending on the kind of questions that we are interested in. Generally, the sample space chosen for a probabilistic model must be __collectively exhaustive__, in the sense that no matter what happens in the experiment, we always obtain an out- come that has been included in the sample space. In addition, the sample space should have enough detail to distinguish between all outcomes of interest to the modeler, while avoiding irrelevant details.

##### Sequential Models

Many experiments have an inherently sequential character, such as for example tossing a coin three times, or observing the value of a stock on five successive days, or receiving eight successive digits at a communication receiver. It is then often useful to describe the experiment and the associated sample space by means of a __tree-based sequential description__.

##### Probability Laws

Suppose we have settled on the sample space Ω associated with an experiment. Then, to complete the probabilistic model, we must introduce a __probability law__. Intuitively, this specifies the “likelihood” of any outcome, or of any set of possible outcomes (an event, as we have called it earlier). More precisely, the probability law assigns to every event A, a number P(A), called __the probability of A__, satisfying the following axioms.

> Probability Axioms
> 1. (Nonnegativity) P(A) ≥ 0, for every event A.
> 2. (Additivity) If A and B are two disjoint events, then the probability of their union satisfies
  P(A ∪ B) = P(A) + P(B).
  Furthermore, if the sample space has an infinite number of elements and A1 , A2 , . . . is a sequence of disjoint events,   then the probability of their union satisfies
  P(A1 ∪A2 ∪···)=P(A1)+P(A2)+···
> 3. (Normalization) The probability of the entire sample space Ω is equal to 1, that is, P(Ω) = 1.

##### Discrete Models

> __Discrete Probability Law__:
  If the sample space consists of a finite number of possible outcomes, then the probability law is specified by the probabilities of the events that consist of a single element. In particular, the probability of any event {s1 , s2 , . . . , sn } is the sum of the probabilities of its elements:
  ``` P {s1,s2,...,sn} = P {s1} +P {s2} +···+P {sn} .```

In the special case where the probabilities P {s1}), . . . , P({sn} are all the same (by necessity equal to 1/n, in view of the normalization axiom), we obtain the following.

> Discrete Uniform Probability Law
  If the sample space consists of n possible outcomes which are equally likely (i.e., all single-element events have the same probability), then the proba- bility of any event A is given by ```P(A) = Number of elements of A / n ```.
  
##### Continuous Models

Probabilistic models with continuous sample spaces differ from their discrete counterparts in that the probabilities of the single-element events may not be sufficient to characterize the probability law. 

##### Properties of Probability Laws

```
Consider a probability law, and let A, B, and C be events. 
(a) If A⊂B, then P(A)≤P(B).
(b) P(A∪B)=P(A)+P(B)−P(A∩B).
(c) P(A∪B)≤P(A)+P(B).
(d) P(A∪B∪C)=P(A)+P(Ac ∩B)+P(Ac ∩Bc ∩C).
```

## 1.3 CONDITIONAL PROBABILITY


