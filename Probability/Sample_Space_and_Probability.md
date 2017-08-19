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

In more precise terms, given an experiment, a corresponding sample space, and a probability law, suppose that we know that the outcome is within some given event B. We wish to quantify the likelihood that the outcome also belongs to some other given event A. We thus seek to construct a new probability law, which takes into account this knowledge and which, for any event A, gives us the __conditional probability__ of A given B, denoted by P(A | B).

This argument suggests that an appropriate definition of conditional probability， is
```P(A|B)= P(A ∩ B) / P(B)```

> __Properties of Conditional Probability__
  The conditional probability of an event A, given an event B with P(B) > 0, is defined by ```P(A|B)= P(A ∩ B) / P(B)```,and specifies a new (conditional) probability law on the same sample space Ω. In particular, all known properties of probability laws remain valid for conditional probability laws.
  Conditional probabilities can also be viewed as a probability law on a new universe B, because all of the conditional probability is concen- trated on B.
  
##### Using Conditional Probability for Modeling

When constructing probabilistic models for experiments that have a sequential character, it is often natural and convenient to first specify conditional prob- abilities and then use them to determine unconditional probabilities. The rule P(A∩B) = P(B)P(A | B), which is a restatement of the definition of conditional probability, is often helpful in this process.

We have a general rule for calculating various probabilities in conjunction with a tree-based sequential description of an experiment. In particular:

* (a) We set up the tree so that an event of interest is associated with a leaf. We view the occurrence of the event as a sequence of steps, namely, the traversals of the branches along the path from the root to the leaf.  
* (b) We record the conditional probabilities associated with the branches of the tree.  
* (c) We obtain the probability of a leaf by multiplying the probabilities recorded along the corresponding path of the tree.  
  
In mathematical terms, we are dealing with an event A which occurs if and only if each one of several events A1,...,An has occurred, i.e., A = A1 ∩A2 ∩ · · · ∩ An. The occurrence of A is viewed as an occurrence of A1, followed by the occurrence of A2, then of A3, etc, and it is visualized as a path on the tree with n branches, corresponding to the events A1, . . . , An. The probability of A is given by the following rule.

__Multiplication Rule.__ Assuming that all of the conditioning events have positive probability, we have
  
![alt](http://www.math.uwaterloo.ca/~dlmcleis/s230/graphics/s230_slidesc1_4__144.png)



## 1.4 TOTAL PROBABILITY THEOREM AND BAYES’ RULE

##### Total Probability Theorem

In probability theory, the __aw (or formula) of total probability__ is a fundamental rule relating __marginal probabilities__ to __conditional probabilities__. It expresses the total probability of an outcome which can be realized via several distinct events—hence the name.



##### Bayes’ Rule
In probability theory and statistics, Bayes’ theorem (alternatively Bayes’ law or Bayes' rule) describes the probability of an event, based on prior knowledge of conditions that might be related to the event.

Bayes' theorem is stated mathematically as the following equation:

![alt](https://wikimedia.org/api/rest_v1/media/math/render/svg/b1078eae6dea894bd826f0b598ff41130ee09c19)

where A and  B are events and P(B) != 0.

* P(A) and P(B) are the probabilities of observing A and  B without regard to each other.
* P(A) and { P(B) are the probabilities of observing A and B without regard to each other.
* P(A / B), a conditional probability, is the probability of observing event A given that  B is true.
  
Bayes’ rule is often used for __inference__. There are a number of “causes” that may result in a certain “effect.” We observe the effect, and we wish to infer the cause. The events A1, . . . , An are associated with the causes and the event B represents the effect. The probability P(B | Ai) that the effect will be observed when the cause Ai is present amounts to a probabilistic model of the cause-effect relation. Given that the effect B has been observed, we wish to evaluate the (conditional) probability P(Ai | B) that the cause Ai is present.

## 1.5 INDEPENDENCE

We have introduced the conditional probability P(A|B) to capture the partial information that event B provides about event A. An interesting and important special case arises when the occurrence of B provides no information and does not alter the probability that A has occurred, i.e., P(A|B) = P(A).

When the above equality holds, we say that A is independent of B. Note that by the definition P(A | B) = P(A ∩ B)/P(B), this is equivalent to P(A ∩ B) = P(A)P(B).

We adopt this latter relation as the definition of independence because it can be used even if P(B) = 0, in which case P(A|B) is undefined. The symmetry of this relation also implies that independence is a symmetric property; that is, if A is independent of B, then B is independent of A, and we can unambiguously say that A and B are __independent events__.

##### Conditional Independence

We noted earlier that the conditional probabilities of events, conditioned on a particular event, form a legitimate probability law. We can thus talk about independence of various events with respect to this conditional law. In particular, given an event C, the events A and B are called conditionally independent if ```P(A ∩ B|C) = P(A|C)P(B|C)```.

##### Independent Trials and the Binomial Probabilities

If an experiment involves a sequence of independent but identical stages, we say that we have a sequence of independent trials. In the special case where there are only two possible results at each stage, we say that we have a sequence of independent __Bernoulli trials__. The two possible results can be anything, e.g., “it rains” or “it doesn’t rain,” but we will often think in terms of coin tosses and refer to the two results as “heads” (H) and “tails” (T).

Let us now consider the probability, p(k) = P(k heads come up in an n-toss sequence), which will play an important role later. We showed above that the probability of any given sequence that contains k heads is pk (1 − p)n−k , so we have

## 1.6 COUNTING

In what follows, we will focus primarily on two types of counting arguments that involve the selection of k objects out of a collection of n objects. If the order of selection matters, the selection is called a __permutation__, and otherwise, it is called a __combination__. 


We start with n distinct objects, and let k be some positive integer, with k ≤ n. We wish to count the number of different ways that we can pick k out of these n objects and arrange them in a sequence, i.e., the number of distinct k-object sequences. We can choose any of the n objects to be the first one. Having chosen the first, there are only n − 1 possible choices for the second; given the choice of the first two, there only remain n − 2 available objects for the third stage, etc. When we are ready to select the last (the kth) object, we have already chosen k − 1 objects, which leaves us with n − (k − 1) choices for the last one. By the Counting Principle, the number of possible sequences, called __k-permutations__.


To count the number of combinations, note that selecting a k-permutation is the same as first selecting a combination of k items and then ordering them. Since there are k! ways of ordering the k selected items, we see that the number of k-permutations is equal to the number of combinations times k!. Hence, the number of possible combinations, is given by 

![alt](http://ictedusrv.cumbria.ac.uk/maths/SecMaths/U3/images/pic057.gif)

* Permutations of n objects: n!
* k-permutations of n objects: n!/(n − k)!

## 1.7 SUMMARY AND DISCUSSION

A probability problem can usually be broken down into a few basic steps:
1. The description of the sample space, that is, the set of possible outcomes of a given experiment.
2. The (possibly indirect) specification of the probability law (the probability of each event).
3. The calculation of probabilities and conditional probabilities of various events of interest.

The probabilities of events must satisfy the nonnegativity, additivity, and nor- malization axioms. In the important special case where the set of possible out- comes is finite, one can just specify the probability of each outcome and obtain the probability of any event by adding the probabilities of the elements of the event.

Conditional probabilities can be viewed as probability laws on the same sample space. We can also view the conditioning event as a new universe, because only outcomes contained in the conditioning event can have positive condi- tional probability. Conditional probabilities are derived from the (unconditional) probability law using the definition P(A | B) = P(A ∩ B)/P(B). However, the reverse process is often convenient, that is, first specify some conditional proba- bilities that are natural for the real situation that we wish to model, and then use them to derive the (unconditional) probability law. Two important tools in this context are the multiplication rule and the total probability theorem.

We have illustrated through examples three methods of specifying proba- bility laws in probabilistic models: 
(1) The counting method. This method applies to the case where the num- ber of possible outcomes is finite, and all outcomes are equally likely. To calculate the probability of an event, we count the number of elements in the event and divide by the number of elements of the sample space.
(2) The sequential method. This method applies when the experiment has a sequential character, and suitable conditional probabilities are specified or calculated along the branches of the corresponding tree (perhaps using the counting method). The probabilities of various events are then obtained by multiplying conditional probabilities along the corresponding paths of the tree, using the multiplication rule.
(3) The divide-and-conquer method. Here, the probabilities P(B) of vari- ous events B are obtained from conditional probabilities P(B|Ai), where the Ai are suitable events that form a partition of the sample space and have known probabilities P(Ai). The probabilities P(B) are then obtained by using the total probability theorem.




