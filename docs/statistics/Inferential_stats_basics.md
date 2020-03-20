title: Inferential Stats - Basics
author: hazeez
date: Mar 18, 2020
date_modified:

# Inferential Statistics

In real-life situations, we may not be able to know the entire population; in which case, we use the _known_ random sample to extract information about the _unknown_ population from which the sample is drawn.

To put it simply, using the sample to come up with an estimation of the population is called as _Inferential statistics_

## Parameter and Statistic

A numerical measure of a population is called a **_population parameter_** or more simply, a **_parameter_**.

Examples of parameters are population mean, population variance, population standard deviation, etc.

A numerical measure of the sample is called a **_sample statistic_**, or simply a **_statistic_**.

Examples of sample statistics are the sample mean, sample variance, sample standard deviation, etc.

In inferential statistics, population parameters are _estimated_ by sample statistics.

When a simple statistic is used to estimate the population parameter, the statistic is called an **_estimator_** of the parameter.

### Notations of parameter and statistic

| Population | Symbol  | | Sample|Symbol|
|--|--|--|--|--|
| Mean | $\mu$  ||Mean|$x$|
| Variance| $\sigma^2$  ||Variance|$s^2$|
| Std deviation | $\sigma$ ||Std deviation|$s$|

To summarize, we have the following relationships between a sample statistic and a population parameter

$$
\bar{x} \space \space \space \overrightarrow{estimates} \space \space \space \mu \\
\\
S^2 \space \space \space \overrightarrow{estimates} \space \space \space  \sigma^2 
$$

i.e the sample mean estimates the population mean and the sample variance estimates the population variance.

## Confidence levels and confidence intervals

To understand confidence level and confidence intervals, we will need to understand what a population distribution and a sampling distribution is.

### Population distribution

The population is the _entire set of values/data points_ that we are interested in. For example, if we know the age of all Indian residents, it is called the population.

The population characteristics are mean $\mu$, standard deviation $\sigma$, median, percentiles, etc.

![](https://i.imgur.com/walJM6I.png)

### Sampling distribution

The sample is a _subset of the population_ which is used to estimate the population characteristic. 

This sample has a few characteristics like mean $\bar{x}$, standard deviation $s$, etc. 

Samples are used to draw inferences about the population. This is done by drawing samples and computing the sample statistics. When the sample statistics are plotted, the distribution (represented as a histogram) is called the sampling distribution. 

!!! Note
	The sampling distribution is also called as theoretical distribution

![](https://i.imgur.com/Y8TyQi7.png)

#### How is a sampling distribution plotted?

From the population, we take $N$ samples of $n$ size and compute the mean. Then we compute the frequency of these means and plot a histogram that would give the sampling distribution.

![](https://media.giphy.com/media/VHZTZYWw8Zon8dWhe0/giphy.gif)

!!! Note
	If the population is normally distributed, then the sampling distribution will also be normally distributed.

### Standard error

The standard error $SE$ is the standard deviation of the sampling distribution

### Standard error of the mean

The standard error (or deviation) of the mean can be expressed as

$$
SE = \sigma_{\bar{x}} = \frac{\sigma}{\sqrt n}
$$

where

$\sigma$ is the standard deviation of the population

$n$ is the size of the sample

Since the standard deviation of the population is rarely known, the standard error of the mean is usually estimated as the sample standard deviation divided by the square root of the sample size i.e.

$$
SE = \sigma_{\bar{x}} \approx \frac{s}{\sqrt n}
$$

where

$s$ is the sample standard deviation
$n$ is the size of the sample.

### Confidence interval

When we use samples to project population estimates, we cannot be CERTAIN that it will be accurate. There is an amount of uncertainty that needs to be factored in/calculated.

So we come up with a range and state that the population parameter (e.g. population means $\mu$) would fall within this range. This is called the **confidence interval**

#### Definition

A confidence interval is the *range of numbers* that is believed to include an unknown population parameter.

#### Confidence level

Let's recall the empirical split.

!!! Note "Recall Empirical rule/split"
	
	The empirical rules state that for a normal distribution, nearly all of the data will fall within three standard deviations of the mean.
	
	- 68% data will fall within 1 standard deviation
	- 95% data will fall within 2 standard deviation
	- 99.7% data will fall within 3 standard deviation
	
	This rule is called as the **3 sigma rule** or **68-95-99.7 rule** 
	
	![](https://i.imgur.com/GMNSUCq.png)

We know that if a population is normally distributed, then 68% of the data will fall under 1 standard deviation. This also means that we are 68% confident that the population mean is within the 1 standard deviation range. Similarly, a 95% confidence level means that the population mean will be within the 2 standard deviation range.

So confidence levels are expressed as a percentage (for example, a 95% confidence level). It means that should you repeat an experiment or survey over and over again, 95 percent of the time your results will match the results you get from a population.

#### Formula

The formula for computing the confidence interval is

$$
CI = \mu \pm z *SE
$$

where
$\mu$ is the mean, $z$ is the quantile, $SE$ is the standard error

Most of the time, the population mean is not known. In that case, the formula becomes

$$
CI = \bar{x} \pm z *SE
$$

where $\bar{x}$ is the mean of the sampling distribution.

Substituting the standard error formula (mentioned above), we get

$$
CI = \bar{x} \pm z * \frac{\sigma}{\sqrt n}
$$

This would give the confidence interval - the range within which the population parameter would fall.

### Margin of error

The margin of error is the range of the expected variation for a given survey result. If we keep repeating the survey using the same methodology, the results of the survey would fall within that range of variation.

In short, half of the confidence interval is called the margin of error. 

The margin of error (ME) is denoted by the formula $z * SE$ which is 

$$
ME = z * \frac{\sigma}{\sqrt n}
$$

The following image represents the confidence interval and the margin of error in a sampling distribution.

![](https://i.imgur.com/gc1Tobd.png)


### Example

A ==survey== was taken of US companies that do business with firms in India. One of the survey questions was: Approximately how many years has your company been trading with firms in India? A random ==sample of 44 responses== to this question yielded a ==mean of 10.455 years==. Suppose the ==population standard deviation== for this question is 7.7 years, construct a ==90% confidence== interval of the {++mean number of years++} that a company has been trading in India {++for the population++} of US companies trading with firms in India. 

#### Known parameters

$$
n = 44 \\
\bar{x} = 10.455 \\
\sigma = 7.7 \\
confidence \space level = 90%
$$

z value for 90% confidence interval  is 1.64

#### To find: confidence interval that has the population mean

#### Solution approach

We know the formula for the confidence interval 

$$
CI = \bar{x} \pm z * \frac{\sigma}{\sqrt n}
$$

substituting, we get

$$
CI = 10.455 \pm 1.64 * \frac{7.7}{\sqrt 44}
$$

which is 

$$
CI = [8.545 , 12.365]
$$

The analyst is 90% confident that the actual population mean number of trading years of firms would be between 8.545 and 12.365.

![](https://i.imgur.com/eSOZiT4.png)

### Example 2

The lung function in ==57 people== is tested using FEVI (Forced Expiratory Volume in 1 Second) measurements. The ==mean FEVI value for this sample== is 4.062 litres and ==standard deviation==, s is 0.67 litres. Construct the 95% Confidence Interval.

#### Data

|      |      |      |      |      |      |
|------|------|------|------|------|------|
| 2.85 | 3.42 | 3.7  | 4.14 | 4.47 | 4.9  |
| 2.85 | 3.48 | 3.75 | 4.16 | 4.5  | 5    |
| 2.98 | 3.5  | 3.78 | 4.2  | 4.5  | 5.1  |
| 3.04 | 3.54 | 3.83 | 4.2  | 4.56 | 5.1  |
| 3.1  | 3.54 | 3.9  | 4.3  | 4.68 | 5.2  |
| 3.1  | 3.57 | 3.96 | 4.3  | 4.7  | 5.3  |
| 3.19 | 3.6  | 4.05 | 4.32 | 4.71 | 5.43 |
| 3.2  | 3.6  | 4.08 | 4.44 | 4.78 | 3.3  |
| 3.69 | 4.1  | 4.47 | 4.8  | 3.39 | 3.7  |
| 4.14 | 4.47 | 4.8  |      |      |      |

#### Known parameters

$$
\bar{x} =  4.062 \\
s = 0.67 \\
n = 57
$$

The z value for a 95% confidence level is 1.96

#### Solution approach

We know the formula for the confidence interval 

$$
CI = \bar{x} \pm z * \frac{\sigma}{\sqrt n}
$$

substituting, we get

$$
CI = 4.062 \pm 1.96 * \frac{0.67}{\sqrt 57}
$$

$$
CI = [3.89, 4.23]
$$

!!! Note "Additional material"

	What happens to confidence interval as confidence level changes? Refer to [this article](../../exercises/exercise06) for the answer.

## Z-Score

Z-score denotes the _number of units of standard deviation from the mean_ the data point is.

A Z-score will also help in finding the probability i.e. area under the curve of where the data point would fall in the normal distribution

More info [here](../../exercises/exercise05)

#### Formula

Z-score is derived using the formula

$$
z = \frac{x - \mu}{\sigma}
$$

where x is the data point we are interested in, $\mu$ is the mean and $\sigma$ is the standard deviation.

### Example

Take a look at the weight of newborn babies. Suppose that the ==mean
weight of newborns is 7.5 pounds== and the ==standard deviation is 1.25 pounds==. Say you’re interested in {++determining the probability++} that a newborn weighs less than 6 pounds. How do you do that?

#### Known parameters

$$
\mu = 7.5 \\
\sigma = 1.25 \\
data \space  point \space x = 6
$$

To find the probability of the new-born weighing less than 6 pounds

#### Solution approach

We know the formula of the z-score.

$$
z = \frac{x - \mu}{\sigma}
$$

substituting the values, we get

$$
z = \frac{6 - 7.5}{1.25} = -1.20
$$

The graph would look like the below

![](https://i.imgur.com/jADvfZx.png)

To find the probability, the z-table is used. 

!!! Note
	There are two Z-tables - one for a positive value of Z and other for a negative value of Z.

Here, the value of Z is -1.20 which is on the negative side and hence, we will be using the negative z table.

-1.20 is read in the table as -1.2 in the rows and 0 in the columns - highlighted below. 

The probability that the baby is born less than 6 pounds is 0.1150 or 11.5%. [See image below]

![](https://i.imgur.com/WYtLrLQ.png)

#### What is the probability that the new-born baby might weigh more than 10 pounds?

Let's visualize it.

![](https://i.imgur.com/FaLRkI1.png)

#### Solution approach

Let's compute the Z-score

We know the formula of the z-score.

$$
z = \frac{x - \mu}{\sigma}
$$

substituting the values, we get

$$
z = \frac{10 - 7.5}{1.25} = 2.0
$$

The graph would look like the below - the shaded area is the probability of newborn weighing **less than 10 pounds**

Looking into the z-table for positive scores, we get the probability value as 0.97725 i.e 97.7% of the newborn is less than or equal to 10 pounds.

The question is about the probability of babies weighing **more than 10 pounds**

![](https://i.imgur.com/lgbC0Fg.png)

To find that, we have to subtract the babies weighing less than or equal to 10 pounds from 1 i.e. 

_babies weighing more than 10 pounds = 1 - babies weighing less than 10 pounds_

!!! Note
	We are subtracting from 1 because the total probability is equal to 1

So we get

Babies weighing more than 10 pounds $= 1 - 0.9772 = 0.0228$ or $2.2\%$

### Summary

To summarize, we started with what is inferential statistics - using the samples to estimate the population, what is a parameter and a statistic, confidence interval and confidence level, standard error and the margin of error, Z- scores and a few examples in each of these.

#### Next post

[Hypothesis Testing](../hypothesis_testing_01)
