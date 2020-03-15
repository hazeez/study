title: Probability theory
author: hazeez
date: Mar 15, 2020
date_modified: Mar 15, 2020

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

Denoted by $A \bigcap B$, the intersection is the set containing all elements that are members of both A and B.

![](https://i.imgur.com/lgdCCj2.png)

#### Union of a set

Denoted by $A \bigcup B$, is the set containing all the elements that are members of both A and B

![](https://i.imgur.com/BttCVn5.png)

#### Experiment and Outcome

Experiment is a process that leads to one or several possible outcomes.

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

		Note: There are 4 Ace's in a deck of cards - Spade, Club, Heart and Diamond

!!! Practice

	Roulette is a popular casino game. As the game is played in Las Vegas or Atlantic City, the roulette wheel has 36 numbers, 1 through 36, and the number 0 as well as the number 00 (double zero). What is the probability of winning on a single number that you bet?

	Solution:

		total elements in the set = 36 + 2 (0 and 00) = 38

			Probability of winning a single number = $\frac{1}{38}$

## Basic rules of probability

#### The range of values

For any event A, the probability $P(A)$ lies between 0 and 1.
i.e. $0 \le P(A) \le 1$

When a probability cannot occur, the probability is zero. 

!!! Example

	What is the probability of drawing a green card from the deck of cards? It's 0 as the deck of cards have only red / black cards.

When a probability is certain to occur, the probability is one.

#### Rule of complements

Probability of a complement is $P(\bar{A}) = 1 - P(A)$

!!! Example

	The probability of rain tomorrow is 0.3. This means the probability of no rain is 1 - 0.3 = 0.7

#### Rule of unions

The rule of unions:

$P(A \bigcup B) = P(A) + P(B) - P(A \bigcap B)$

!!! Example

	The probability of an Ace in a deck of cards is $\frac{4}{52}$ and the probability of a heart in a deck of cards is $\frac{13}{52}$. The probability of an ace with heart is $\frac{1}{52}$

	So $P(A \bigcup \heartsuit) = \frac{4}{52} + \frac{13}{52} - \frac{1}{52} = \frac{16}{52}$
