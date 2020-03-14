title: Test statistic - Z & t
author: hazeez
date: Mar 12, 2020
date modified: Mar 15, 2020


# Test statistic - Z & t

> In the [previous article](../hypothesis_testing_02), we used test statistic as a value to compare against the critical value. This helps us to accept or reject our null hypothesis.
> In this article, we will see what is a test statistic and how to compute it.

!!! Note
	We are in the fourth step of the hypothesis testing process 
	- Find the test statistic

## What is a test statistic?

A test statistic is used in a hypothesis test to decide to support or reject a null hypothesis. A test statistic is a number that is calculated from a sample and is compared with the null hypothesis.

So what does this mean?

We know that for the population we have parameters and for sample, we have statistics. i.e. any value that represents the population is called as _parameter_ and any value that represents sample is called as a _statistic_

We use this sample and come up with a value (statistic). This is called the test statistic.

## Methods of finding the test statistic

There are various methods/tests for finding the test statistic. Usually, the following four methods are used.

- _Z_ test
- _t_ test
- Chi-squared test ($\chi^2$)
- F test

In this article, we will cover the _Z_ test and _t_ test.

We have these tests - how are they different? 

When the null hypothesis is about the **mean** of the population, the _Z_ test or the _t_ test is used.

When the null hypothesis is about the **variance** of the population, the $\chi^2$ (chi-square) test and the _F_ test is used.

Let us see the _Z_ test first.

## Z test

### Assumptions of a Z test

Z test is used when the following conditions are met.

1. The sample size `n` should be greater than 30 i.e. $n > 30$
2. The population standard deviation should be known
3. The variable should be continuous (remember, this is a continuous sampling distribution)

### Formula for Z test

The test statistic for _Z_ test is represented as **_test Z_**

The formula for finding the test statistic in a _Z_ test is

$$
\textrm {test}\space Z = \frac{\bar{x} - \mu} {\sigma / \sqrt n}
$$

where $\bar{x}$ is the sample mean, $\mu$ is the population mean, $\sigma$ is the population standard deviation and  $n$ is the number of samples.

### Example

Let's say the null and the alternate hypothesis are

$$
\mathbf{H}_\mathbf{0} : \mu \ge 1000 \\
\mathbf{H}_\mathbf{1} : \mu	< 1000
$$

and the population standard deviation $\sigma$ is known and a random sample of size $n$ = 30 is taken, then the test statistic of $Z$ would be

$$
test\space Z = \frac{\bar{x} - 1000}{\sigma / \sqrt 30}
$$

#### Let's check our understanding with a detailed example

> Let's highlight the keywords along with the problem statement

An automatic bottling machine fills cola into 2-liter (`2,000`- cubic cm) bottles. A consumer advocate wants to ==test the null hypothesis that the average amount filled by the machine into a bottle is at least `2,000` cubic cm==. A random ==sample of`40` bottles== coming out of the machine was selected and the exact contents of the selected bottles are recorded.
The ==sample mean was `1,999.6` cubic cm==. The ==population standard deviation== is known from past experience to be 1.30 cubic cm. Test the null hypothesis at an ==$\alpha$ of 5%.==

Let's write the values that have been provided

$\mu = 2000; \space n = 40; \space \bar{x} = 1999.6;\space\sigma=1.30; \space \alpha = 5%$

Let's try to follow the hypothesis test process

1. State the null and the alternate hypothesis
2. Choose the level of significance
3. Find the critical value
4. Find the test statistic
5. Draw the conclusion

#### 1. Stating the null and the alternate hypothesis

$$
\mathbf{H}_\mathbf{0}: \mu \ge 2000 \\
\mathbf{H}_\mathbf{1}: \mu < 2000 
$$

We see the sign of the alternate hypothesis and it is `<` (less than symbol) which means the test is a ==one-tailed lower-tail test.==

#### 2. Choose the level of significance

The level of significance provided is $\alpha = 5$%. 
So the confidence level is , 1 - $\alpha\space = 95$% 

#### 3. Find the critical value

The corresponding Z score (critical value) is $z_c = -1.64$ 
Here the `-` (negative) sign implies that it is a lower tail test.

!!! Note
	The Z score for 95% is 1.64 but, since this is a lower-tailed test, we take the Z score as -1.64

The rejection region is highlighted in the graph below

![](https://i.imgur.com/1zzXU27.png)

#### 4. Find the test statistic

Here the sample is $n = 40$ which means it confirms to the first condition of the $Z$ test mentioned above

Second, the population standard deviation is known - which means we can use the $Z$ test to find the test statistic

The formula for computing the $Z$ score is

$$
\textrm {test}\space Z = \frac{\bar{x} - \mu} {\sigma / \sqrt n}
$$

When we substitute the values, we get 

$$
\textrm {test}\space Z = \frac{1999.6 - 2000} {1.30 / \sqrt 40}
$$

which yeilds the result $\textrm {test} \space z$ = -1.95

When we plot it in the graph, the graph would look like the below image

![](https://i.imgur.com/XIaMrcJ.png)


The test statistic $\textrm{test} \space z$ falls within the rejection range. Hence the null hypothesis will be rejected.

#### 5. Drawing the conclusion

The hypothesis that the average amount filled by the cola machine into a cola bottle is less than `2,000` cubic cm and hence, it is rejected.

> To sum up, the Z test is used to calculate the test statistic when the null hypothesis is about the means of the population and it satisfies the assumption mentioned above.

## 't' test or Student 't' test

We saw that the 'Z' test is applicable when the sample size is greater than 30 i.e. `n>30`. There arises a logical question as to what test is to be done when the sample size is less than 30 i.e. `n<30`. We use the 't' test for computing the test statistic for null hypothesis testing.


### Assumptions of a 't' test

$t$ test is used when the following conditions are met.

1. The sample size `n` should be less than 30 i.e. $n < 30$
2. The population standard deviation is not known irrespective of the sample size
3. The population is normally distributed


### Formula for 't' test

$$
t \space statistic \space (or \space t\space score), t= \frac{\bar{x} - \mu}{s /\sqrt n}
$$

where $\bar{x}$ is the sample mean, $\mu$ is the population mean, $s$ is the sample standard deviation[^1] and  $n$ is the number of samples.
[^1] Since we don't know the population standard deviation in a 't' test, we use the sample standard deviation

#### Characteristics of the 't' distribution

- it has degrees-of-freedom parameter $df$
- it is symmetric and bell-shaped
- has wider tails than the Z distribution

!!! Extra_research

	Why does a $t$ distribution has wider tails than the Z distribution?
	
	In a $t$ distribution, the population standard deviation ($\sigma$) is not known and only the sample standard deviation ($s$) is known. We know that by using the sample standard deviation, we cannot accurately project the population variance. Hence, to accommodate the level of _uncertainity_ in computing the population variance, it has wider tails.
	
	As the degree of freedom ($df$) increases, the t-distribution approaches the 'Z' distribution
	
	![](https://i.imgur.com/dpRUXEb.png)
	
	The 't' distribution with infinite degrees-of-freedom is called as the _standard normal distribution._

### Confidence interval to estimate the population mean

As the population standard deviation, $\sigma$ is not known in a $t$, we will not able to estimate the population mean $\mu$ - but, we can find the range (confidence interval) of the population mean $\mu$

The formula for computing the confidence interval to estimate $\mu$ is

$$
\bar{x} - t_{n-1,\frac{\alpha}{2}} \frac{s}{\sqrt n} \le \mu \le \bar{x} + t_{n-1,\frac{\alpha}{2}} \frac{s}{\sqrt n}
$$

where $\bar{x}$ is the sample mean, $t$ is the test statistic of the $t$ distribution, $n-1$ is the degree of freedom, $\alpha$ is the level of significance, $S$ is the sample standard deviation, $n$ is the number of samples.

#### Why $\frac{\alpha}{2}$ ?
	
In a confidence interval, the area is symmetrically distributed between the two tails. 

![](https://i.imgur.com/Yq74Mrd.png)

### Example

A stock market analyst wants to estimate the average return on a certain stock. A random sample of 15 days yields an average (annualized) return of $\bar{x}$ 10.37% and a standard deviation of s $=$ 3.5%. Assuming a normal population of returns, give a 95% confidence interval for the average return on this stock.

#### What we know here?

Sample of 15 days i.e. $s = 15$ (since sample is less than 30, _t_ test is to be used)
We need to use _t_ distribution with $n-1$ degrees of freedom. So, $df = 14$.
Sample standard deviation $s = 3.5$
Sample mean $\bar{x} = 10.37$
Confidence level is 95%. So the level of significance deduced is 5%.

!!! Remember the formula
	confidence level = 1 - $\alpha$ which means
	$\alpha$ = 100 - confidence level

#### Solution

We know the formula for the confidence interval of the _t_ distribution is 

$$
\bar{x} - t_{n-1,\frac{\alpha}{2}} \frac{s}{\sqrt n} \le \mu \le \bar{x} + t_{n-1,\frac{\alpha}{2}} \frac{s}{\sqrt n}
$$

If we substitute the values, we get

$$
10.37 - t_{14,0.025} \frac{3.5}{\sqrt 15} \le \mu \le 10.37 + t_{14,0.025} \frac{3.5}{\sqrt 15}
$$

From the _t_ tables, we can find the _t_ statistic value for $df = 14$ and $\alpha /2 = 0.025$ is

$$
t_{14,0.025} = 2.145
$$

See below image for finding the t value for $df = 14$ and $\alpha = 0.025$

![](https://i.imgur.com/U4arKUU.png)

Substituting in the formula, we get

$$
10.37 - 2.145 \frac{3.5}{\sqrt 15} \le \mu \le 10.37 + 2.145 \frac{3.5}{\sqrt 15}
$$

the confidence interval range is $[8.43, 12.31]$. This is represented as 

$$
CI(0.05) = [8.43, 12.31]
$$

Thus, the analyst may be 95% sure that the average annualized return on the stock is anywhere from 8.43% to 12.31%.

### Degree of Freedom

Degrees of freedom refers to the maximum number of logically independent values in a data sample which have the freedom to vary within. What does that mean?

We will take an example and try to understand.

#### Example

Let us consider that we have a sample of 3 values 

$$
{5, x , 15}
$$

 and the mean of all the values is 10. 

!!! Note
	$x$ is unknown here

It is easy to deduce that the value of $x$ would be 10 as the mean of these 3 values has to equate to 10.

But, let's say 2 values from this sample are not known, 

$$
{5, x, y}
$$

!!! Note
	 ($x, y$ are unknown) 

with the same mean 10, then we cannot be sure about the exact values of $x$ and $y$.

It could be any values of these values - (10, 15), (15, 10), (5, 20), (20, 5) or even (1, 24).

So we cannot determine the exact value of these variables $x$ and $y$.

These 2 values have the freedom to vary. So, the degree of freedom ($df$) of this sample data of size 3 is 2.

#### Formula

$$
df = n – 1
$$

where $df$ is the degree of freedom and $n$ is the  sample size

### Application of t-test

Your company wants to improve sales. Past sales data indicate that the average sale was $100 per transaction. After training your sales force, recent sales data (taken from a sample of 25 salesmen) indicates an average sale of $130, with a standard deviation of $15. Did the training work? Test your hypothesis at a 5% alpha level.

#### What is given?

From the problem, first, we need to understand if the given problem belongs to which category of tests - Z or t.

The average sale is provided $\mu	= 100$. Sample is $n = 25$.
Recent sales data (sample)  is given - ie. average sale $\bar{x} =  130$.
Sample standard deviation $s = 15$.
Level of significance = 5% or 0.05

_Since the sample size is less than 30 and we don't know the population standard deviation, we will go with the t test_

#### Solution Approach

Did the training work? 
In other words, is there an increase in sales after the training is provided.

#### Hypothesis testing steps

We know the hypothesis testing steps 

1. State the null and the alternate hypothesis

	$$
		\mathbf{H}_\mathbf{0}: \mu = 100 \\
		\mathbf{H}_\mathbf{1}: \mu > 100
	$$

	Since the symbol of the alternate hypothesis is greater than, it is a _right-tailed_ test.

2. Find the level of significance.
	
	Here the level of significance is provided - which is $\alpha = 0.05$

3. Find the critical value

	Since this is a t test, we need to use the t-table to find the critical value.
	The t-table has the degree of freedom and corresponding level of significance to provide the critical value.

	Here the degree of freedom $df = n - 1$ which is $25 - 1 = 24$

	Looking into the critical table for $df = 24$ and $\alpha =  0.05$, we get the critical value $t_c = 1.711$ (see figure below)

	![](https://i.imgur.com/SAImuwn.png)


4. Find the test statistic

	We know the formula for the _t_ test is 

	$$
	t_{score} = \frac{\bar{x} - \mu}{s / \sqrt n }
	$$

	Substituting the above values, we get 

	$$
	t_{score} = \frac{130 - 100}{15 / \sqrt 25}
	$$

	which gives us the $t_{score} = 10$

5. Drawing the conclusions

	We see that the $t_{score}$ falls beyond the rejection region and hence the null hypothesis is rejected.

	![](https://i.imgur.com/9muLuQb.png)

	This means to say that indeed the average sales increased after the training.

## Summary

In this article, we saw what a test statistic is!, the different types of tests, when to use _Z_ test and _t_ test and their respective formulas. In the end, we saw what is the degree of freedom along with an application of t-test using an example.

We also got more familiar with the hypothesis testing process and following it would help us accept or reject the null hypothesis in a logical manner.
