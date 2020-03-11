title: Hypothesis Test Process
author: hazeez
date: Mar 12, 2020

# Hypothesis Tests

> In the [previous article](..\hypothesis_testing_01), we got introduced to the concept of hypothesis - null hypothesis and the alternate hypothesis. We concluded with how the _p-value_ is compared with the level of significance to either accept or reject the null hypothesis.
> We will keep _p-value_ aside at the moment and will later see how it is calculated; less we know - less we are confused.


## Hypothesis test steps

Just to recap, hypothesis testing is _the process of determining whether a given hypothesis is true or not_

The highlight is on the word **process**. If it is called a process, then there have to be some steps associated with it.

The steps for testing the hypothesis are mentioned below

1. State the null hypothesis  $\mathbf{H}_\mathbf{0}$ and the alternate hypothesis $\mathbf{H}_\mathbf{1}$
2. Choose the level of significance
3. Find critical values
4. Find test statistic
5. Draw your conclusion

Ok. Sounds good! Let us take stock of what knowledge we have already about the above-mentioned steps. 

We know what the null and the alternate hypothesis are, level of significance, and probably presume what draw your conclusion means.

What we don't know about at this point is

- Step 4 - Find critical values and 
- Step 5 - find the test statistic.

Good! Let's see what a critical value is! 

To understand the critical value and critical region, we need to first understand what _one-tailed_ and _two-tailed_ tests are.

## One-Tailed and Two-Tailed Tests

We have already seen tails in statistics - when there is a long tail to the right of a frequency distribution, the data is positively skewed and where is a long tail to the left, the data is negatively skewed.

So it has to do something with the distribution curve? Yes, you are right! 

Let's dive into detail!

### What are tails?

In the day-to-day context, we know a tail is that extra portion that is attached to the body of an animal. 

Similarly, in the context of statistics, tails are that portion that is attached to the side of distribution - see figure below - _the grey area_

![](https://i.imgur.com/o35gMNp.png)

!!! Note
	Distribution does not have to have two tails always. There can be only one tail as well. 

Now that we have seen the tails visually, we understand things better.
But, there are two tails here - do we have names that distinguish between these tails? 

Yes! It's upper tail and lower tail.

The following image shows the lower tail and upper tail respectively.

![](https://i.imgur.com/yvJK9if.png)

#### Upper tail

The upper tail is towards the upper side i.e. the positive side of the graph (see image above). Remember positive values lie on the right of the graph (1, 2, 3, etc). So it is called as "right-tail" also.

#### Lower tail

The lower tail is towards the lower side i.e the negative side of the graph. Hence it is referred to as "left-tail" as well. 

>So if the distribution has just one tail, it can be either an _upper-tail **or** lower-tail_ and if the distribution has two-tails, it will have both _upper-tail **and** lower-tail_.

#### Critical Region / Rejection Region

The region that is shaded in grey i.e. the tail area is called as the **Critical Region** or **Rejection Region**

The following image shows the _rejection region for the lower-tailed graph_

![](https://i.imgur.com/sKoJ8i9.png)

Similarly, the image below depicts the _rejection region for the upper tailed graph_

![](https://i.imgur.com/iH0jI91.png)

The _rejection region for the two-tailed graph_ is shown below

![](https://i.imgur.com/NuHvOL8.png)

So far, so good!?

Now in real-life problems, we will not be given the graph to understand if the tail is towards the left or right or it is two-tailed.

The problem statement will be provided. We need to figure out the hypothesis and then decide if its right-tailed or left-tailed or both!

### One-Tailed tests

One-tailed tests can be either an upper tailed test or a lower tailed test.

How can we spot or understand which tailed-tests the problem we have at hand belong to? Upper tail or lower tail?

Remember in the previous article, we had stated the hypothesis for two examples. Let's revisit those examples.

**Example 1**

My broadband company claims that the minimum internet speed they are providing is 150 Mbps. However, I suspect that they are not providing the promised internet speed.

Let's write the null and alternate hypotheses for this!

$$
	 \mathbf{H}_\mathbf{0}: speed \ge 150 Mbps \\
	  \mathbf{H}_\mathbf{1}: speed < 150 Mbps
$$

What we are trying to prove is our alternate hypothesis with evidence that the speed is less than 150 Mbps.

So we see the symbol of alternate hypothesis i.e - if it is less than `<` 150 Mbps, it is called a _lower tail_ test.

![](https://i.imgur.com/z4RRP87.png)


**Example 2**

The project manager claims that the software defects raised are resolved within 5 business days. I being the quality department manager think it is taking longer to fix the bugs. 

The null and alternate hypothesis is mentioned below

$$
 \mathbf{H}_\mathbf{0}: Resolution\space  period \le 5 days \\
  \mathbf{H}_\mathbf{1}: Resolution\space period > 5 days
$$

We see that the alternate hypothesis is greater than `>` 5 days. Hence, it is an _upper-tail_ test.

![](https://i.imgur.com/026muUN.png)

!!! Important
	The upper-tailed test or lower-tailed test is determined based on the **alternative hypothesis** only and **NOT** the null hypothesis.

> To conclude, one-tailed tests can be either an _upper-tail_ test or a _lower-tail_ test and the test is determined by the _symbol of the alternate hypothesis_ $\mathbf{H}_\mathbf{1}$

### Two-Tailed tests

#### So how does the hypothesis of a two-tailed test look like?

A residential school claims that the average time the students of the school get to do extra-curricular activities is 200 hours per year but, the parents doubt that the students spend so much time.

The null and the alternate hypothesis looks like the below

$$
 \mathbf{H}_\mathbf{0}: \mu	= 200 \space hours \\
  \mathbf{H}_\mathbf{1}: \mu \ne 200 \space hours
$$

Here we see the symbol of the alternate hypothesis is $\ne$ which means the test is a _two-tailed_ test. We don't check for increase or decrease i.e. $\ge$ or $\le$ but, we check for a change in the parameter.

So the critical region / tails are split over both the ends.

Both the ends contain $\alpha/2$, making a total of $\alpha$ - which is the level of significance. Refer to the previous article.

![](https://i.imgur.com/5tayxLc.png)

> Milestone reached: So from the hypothesis statement, we are understanding if the test is either a one-tailed (upper or lower tail) or two-tailed.

> We are still in step 3 - Finding the critical value

Let's understand what a critical value is and then we will see how to compute the critical value.

### Critical value

We know what a critical region or a rejection region is! So critical value should be near or in that critical region.

To take an analogy, the critical values of water - i.e. the boiling point is 100 deg Celcius and the freezing point is 0 deg Celcius. It is an important measure that helps us make important decisions.

#### Definition of critical value

A critical value is a line on a graph that splits the graph into sections. If our test value falls into that region, then you reject the null hypothesis - which means the samples and the evidence we had taken supports the alternate hypothesis

Critical value depicted in the graph below - for lower-tailed graph

![](https://i.imgur.com/aTaG3bX.png)

Similarly, the critical value for the upper-tailed graph is below

![](https://i.imgur.com/mIsCOBT.png)

Critical values for a two-tailed graph is below

In the case of a two-tailed graph, the value that we are computing should be either below or above the critical value for rejecting the null hypothesis.

![](https://i.imgur.com/kHb4sZ1.png)

Ok - now we have visualized what a critical value is. This critical value is nothing but the =='Z' score==

We already know some of the common 'Z' scores.

#### Example of a 'Z' score

Let's say we have a sample normal distribution. We know that as per the empirical split (or rule), 68% lie within the `1` standard deviation from the mean, 95% lie within `2` standard deviation from the mean and 99.7% of the values lie within `3` standard deviations from the mean.

We know that 'Z' score for `+2.0` standard deviation is `1.96` and for `-2.0` standard deviation is `-1.96`. We have used this in several computations in the class. We will see how to compute 'Z' scores in another post.

Let us see how the level of significance ($\alpha$) is used to find the critical value (Z score).

> Level of significance is covered in [this post](../hypothesis_testing_01/#level_of_significance)

### Critical value and level of significance

We use the level of significance ($\alpha$) to determine the critical value. How?

**Example:** 

Determine the critical value at `5%` level of significance. Presume its a ==right-tailed / upper-tailed test==.

We know $\alpha$ = `5%` (see image below to find where level of significance $\alpha$ of 5% falls)
and 1 - $\alpha$ is `95%`

![](https://i.imgur.com/AgZGTmb.png)

We know that `95%` of the values fall within the `2` standard deviation mark and the corresponding the 'Z' score is `1.96`.

So the critical value (_Z_) is `1.96`.

#### So how will we determine if we have to accept or reject the null hypothesis?

> I am quoting a new word _test statistic_ here. We will see what it is and how it is computed in the next post. At the moment, just think of _test statistic_ as a number computed from our samples.

If the test statistic (_test Z_) is less than the critical value (_Z_), we will accept the null hypothesis. In other words, we have not stepped into the rejection region and hence will accept.

$$
test\space Z \le Z : \space accept \space  \mathbf{H}_\mathbf{0} \\
test\space Z > Z : \space reject \space  \mathbf{H}_\mathbf{0}
$$

Let's visualize the above scenario with an example graph!

The below are the  numbers

Critical value _Z_ = `1.96`
Test statistic (_test Z_) = `0.5`

Since the test statistic is less than the critical value, we will accept the null hypothesis $\mathbf{H}_\mathbf{0}$

![](https://i.imgur.com/4AbSXzL.png)

### Summary

In this article, we focussed on the 3rd step of the hypothesis testing process - _Find the critical value_

We started with what are tails, upper tail and lower tail, one-tailed tests and two-tailed tests, critical region / rejection region, critical values and when to accept or reject the null hypothesis.

In the next post, we will explore more on finding the _test statistic_ which is the 4th step of the hypothesis testing process.