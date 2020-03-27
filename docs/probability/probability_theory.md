title: Probability theory
author: hazeez
date: Mar 15, 2020
date_modified:
hero:

# Probability

A probability is a _quantitative measure of uncertainity_. 

## Basic Definitions

#### Set

A set is a collection of elements

#### Empty set

A set containing no elements

#### Universal set

A set containing all elements. Represented by _S_

#### Compliment of a set

The complement of set A is the set containing all the elements in the universal
set S that are not members of set A. Represented by $\bar{A}$

#### Intersection of a set

Denoted by $A \cap B$, the intersection is the set containing all elements that are members present in both A and B.

![](https://i.imgur.com/lgdCCj2.png)

#### Union of a set

Denoted by $A \cup B$, is the set containing all the elements that are members of both A and B

![](https://i.imgur.com/BttCVn5.png)

#### Experiment and Outcome

An experiment is a process that leads to one or several possible outcomes.

An outcome of an experiment is some observation or measurement.

!!! Example

	Drawing a card out of a deck of 52 cards is an experiment. One outcome of the experiment may be that the queen of diamonds is drawn.

#### Sample space

Sample space is the set of all possible outcomes of an experiment.

!!! Example

	The sample space for the experiment of drawing a card out of a deck is the set of all cards in the deck.

#### Event

An event is a subset of a sample space.

!!! Example

	An ace is drawn out of a deck of cards.

#### Probability of event A

$$
P(A) = \frac{n(A)}{n(S)}
$$

where

$n(A)=$ the number of elements in the set of the event A

$n(S)=$ the number of elements in the sample space S

!!! Example

	The probability of drawing an Ace is 
	
	$$
		P(A) = \frac{n(A)}{n(S)} = \frac{4}{52}
	$$

	Note: There are 4 Ace's in a deck of cards - Spade, Club, Heart, and Diamond

!!! Practice

	Roulette is a popular casino game. As the game is played in Las Vegas or Atlantic City, the roulette wheel has 36 numbers, 1 through 36, and the number 0 as well as the number 00 (double zero). What is the probability of winning on a single number that you bet?

	Solution:

	total elements in the set = 36 + 2 (include 0 and 00) = 38

	Probability of winning a single number = $\frac{1}{38}$

## Basic rules of probability

#### The range of values

For any event A, the probability $P(A)$ lies between 0 and 1.
i.e. $0 \le P(A) \le 1$

When a probability cannot occur, the probability is zero. 

!!! Example

	What is the probability of drawing a green card from the deck of cards? 
	
	It's 0 as the deck of cards has only red/black cards.

When a probability is certain to occur, the probability is one.

#### Rule of complements

Probability of a complement is $P(\bar{A}) = 1 - P(A)$

!!! Example

	The probability of rain tomorrow is 0.3. 
	
	This means the probability of no rain is 1 - 0.3 = 0.7

#### Rule of unions

The rule of unions:

$P(A \cup B) = P(A) + P(B) - P(A \cap B)$

!!! Example

	The probability of an Ace in a deck of cards is $\frac{4}{52}$ and the probability of a heart in a deck of cards is $\frac{13}{52}$. The probability of an ace with heart is $\frac{1}{52}$

	So $P(A \cup \heartsuit) = \frac{4}{52} + \frac{13}{52} - \frac{1}{52} = \frac{16}{52}$

### Mutually exclusive events

When the sets corresponding to two events are disjoint (i.e. have not an intersection), the two events are called mutually exclusive or in other words, they can't occur together.

To simplify, events are _mutually exclusive_ if they cannot occur simultaneously.

![](https://i.imgur.com/2UOmVZ4.png)

**Intersection:** For mutually exclusive events A and B: 

$P(A \cap B) = 0$

Since there is no intersection, it is always 0

**Union:** For mutualy exclusive events A and B:

$P(A \cup B) = P(A) + P(B)$

!!! Note

	Since there is no intersection, 

	$P(A \cup B) = P(A) + P(B) - P(A \cap B)$ 

	is reduced to 

	$P(A \cup B) = P(A) + P(B)$

!!! Example

	What is the probability of drawing either a heart or a club?

	The probability of drawing a heart is $\frac{13}{52}$.
	The probability of drawing a club is $\frac{13}{52}$.

	Since they are mutually exclusive,
	
	$P(\heartsuit \cup \clubsuit) = P(\heartsuit) + P(\clubsuit)$ which is 
	
	$\frac{13}{52} + \frac{13}{52} = \frac{26}{52} = \frac{1}{2}$
	
## Conditional probability

The probability depends on information.

Say for example - what is the probability that the company Mannar & Co's stock price would go up?

Well, it would depend on the information we have about the company like it's performance in recent times.

So the probability of the stock price going up depends upon some information. This is called as _conditional probability_

#### Formula

The **_conditional probability_** of an event A given the occurrence of event B is

$$
	P(A|B) = \frac{P(A \cap B)}{P(B)}
$$

The vertical line in P(A|B) is read _given_ or _conditional upon_. 

!!! Example
	
	A consulting firm is bidding for two jobs, one with each of two large multinational corporations. The company executives estimate that the probability of obtaining the consulting job with firm A, event A, is 0.45. The executives also feel that if the company should get the job with firm A, then there is a 0.90 probability that firm B will also give the company the consulting job. What are the company’s chances of getting both jobs?
	
	Solution:
	
	$$
	P(A) = 0.45 \\
	P(B|A) = 0.90
	$$

	We are looking for $P(A \cap B)$ - i.e. chance of getting both jobs

	We know the formula is $P(B|A) = \frac{P(B \cap A)}{P(A)}$

	So the formula becomes, $P(B \cap A) = P(B|A).P(A)$

	which is $0.90 * 0.45 = 0.405$

!!! Note

	Conditional probability is not symmetrical 
	
	$P(A|B) \ne P(B|A)$

## Independence of events

As an example of independent events, consider the following: 

Suppose I roll a single die. What is the probability that the number 6 will turn up? 

The answer is $\frac{1}{6}$. 

Now suppose that I told you that I just tossed a coin and it turned up heads. 

What is now the probability that the die will show the number 6? 

The answer is unchanged, $\frac{1}{6}$, because events of the die and the coin are independent of each other. 

We see that $P(6 | H) = P(6)$

So when do we say that the events are independent of each other?

#### Conditions for the independence of two events A and B

The events are said to be independent when they meet the below conditions:

$$
	P(A|B) = P(A) \\
	P(B|A) = P(B) \\
	and \\
	P(A \cap B) = P(A)P(B)
$$

The first equation $P(A|B)=P(A)$ implies that the probability of A would not be affected by the probability of B as they are both independent. So the probability of A would remain the same.

Similarly, the second equation $P(B|A)=P(B)$ implies that the probability of B would remain the same as B is not affected by the probability of A since both are independent.

The third equation $P(A \cap B)= P(A)P(B)$ is called the _intersection rule for independent events_.

#### Intersection rule for independent events

$P(A \cap B)= P(A)P(B)$

The probability of the intersection of several independent events is just the
product of the separate probabilities.

Let's understand this rule with an example.

!!! Example

	The rate of defects in corks of wine bottles is very high say 75%. Assuming independence, if four bottles are opened, what is the probability that all four corks are defective?

	Solution:
	
	P (all 4 are defective) = 
	P (first cork is defective) * P (second cork is defective) * 
	P (third cork is defective) * P (fourth cork is defective)

	which is equal to
	
	P (all 4 are defective) = 0.75 * 0.75 * 0.75 * 0.75 = 0.316

!!! Tip

	Whenever a random sampling is done, it would mean independence - as the outcome of one event will not be dependent on the outcome of another event.

!!! Question

	What is the difference between a mutually exclusive event and an independent event?

	mutually exclusive - Two events cannot occur at the same time. e.g., the head & tail of a coin cannot occur at the same time. They're dependent in fact.

	independent - Two events can occur at the same time and they are not dependent on each other. e.g., events of tossing a coin & events of rolling a dice at the same time are independent.

## Bayes Theorem

Bayes theorem is a technique for calculating a conditional probability.

### Derivation of Bayes Theorem

We have already seen the conditional probability which is

Equation 1:

$$
	P(A|B) = \frac{P(A \cap B)}{P(B)} \space provided \space that \space P(B) > 0
$$

Equation 2:

This also means that

$$
	P(B|A) = \frac{P(B \cap A)}{P(A)} \space provided \space that \space P(A) > 0
$$

So from equation 2, we can say that (Equation 3)

$$ 
P(B \cap A) = P(B|A)P(A)
$$ 

We also know that 

$$
P(A \cap B) = P(B \cap A)
$$

So substituting the Equation 3 in Equation 1, we get the **Bayes theorem.**

$$
	P(A|B) = \frac{P(B|A).P(A)}{P(B)} \space provided \space that \space P(A), P(B) > 0
$$

### Example

Refer to Example 1 (Elderly fall and death) in this [article](https://machinelearningmastery.com/intuition-for-bayes-theorem-with-worked-examples/) for how to apply the Bayes theorem 

## Summary

In this post, we had seen what probability is, definition of terms used in probability, mutually-exclusive and independent events, conditional probability and then the Bayes theorem.