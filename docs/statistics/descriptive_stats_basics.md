title: Descriptive Statistics
author: hazeez
date: Mar 19, 2020
date_modified:

# Descriptive Statistics

## Statistics Basics

### What is statistics?

A branch of mathematics taking and transforming numbers into useful information for decision-makers.

It originated from the word _Stata_ which means _state_ - i.e. understanding about the state of data.

It is a way to get information from data. Complex data can be easily translated into meaningful information using statistics.

### Example

A college in the US has students from the following countries. Which country is in the majority?

|        |        |         |       |         |         |          |         |       |         |
|--------|--------|---------|-------|---------|---------|----------|---------|-------|---------|
| US     | Canada | China   | US    | India   | England | Mexico   | Japan   | China | Germany |
| China  | China  | Germany | US    | Japan   | India   | US       | China   | India | Japan   |
| US     | Japan  | India   | US    | England | China   | Canada   | US      | India | China   |
| Sweden | Mexico | India   | China | India   | Mexico  | Pakistan | Japan   | China | US      |
| China  | US     | Japan   | China | Japan   | US      | India    | Germany | China | Japan   |

It is very difficult to get that information from this data when presented this way. However, when the same data is converted into meaningful information, conclusions can arrive very easily.

Translating the above table into the below table gives us the answer much faster. This is the use of statistics.

| Count    | Frequency |
|----------|:---------:|
| Canada   | 2         |
| China    | 12        |
| England  | 2         |
| Germany  | 3         |
| India    | 8         |
| Japan    | 8         |
| Mexico   | 3         |
| Pakistan | 1         |
| Sweden   | 1         |
| US       | 10        |

### Example 2

Data can be misleading.

A parent changes the school of their Son who is studying in $11^{th}$ standard since his academic results are not good in $10^{th}$ Standard in his current School. They change Student A from ABC school to XYZ school

The result was different

1. Ranked $15^{th}$ in ABC school
2. Ranked $2^{nd}$ in XYZ school

What's the conclusion? Has the student improved?

Well, it depends on the number of students studying school. It seems that in the XYZ school, only 2 students were studying and hence he came $2^{nd}$. 

Such clarity of information can be obtained via statistics.

The knowledge of statistics allows us to make better sense of the use of numbers.

#### Statistics in a nutshell

The branch of statistics can be summed up as 

1. Collecting data
2. Analyzing data
3. Interpreting data
4. Presenting data

### Statistics classification

Statistics can be classified into two types

#### Descriptive statistics

Presenting, organizing and summarizing data is called _descriptive statistics_

#### Inferential statistics

Drawing conclusions about a population based on data observed in a sample is called as _inferential statistics_

We talked about the population and sample in the definition of the inferential statistics above. What does it mean?

_Population_ is the entire set of data points available e.g. elections, 10-year census.

_Sample_ is a subset of the data points taken from the population. e.g. opinion polls

#### Parameter and Statistic

A _parameter_ is a descriptive measure of the population

e.g. population mean, population variance, population standard deviation, etc

A _statistic_ is a descriptive measure of a sample

e.g. sample mean, sample variance, sample standard deviation, etc.

## Types of variables

Variables are the fancy name of data in statistics.

Variables can be classified as _Qualitative_ or _Quantitative_

![](https://i.imgur.com/auPmmPP.png)

#### Nominal variables

Variables that have a name is called as _nominal_ variables

E.g. Gender (male/female), Ethnicity (Indian, American, Russian), etc

#### Ordinal variables

Variables that are based on order/rank

E.g. Movie ratings (1 star to 5 stars), Fortune 50 rankings, etc.

#### Discrete variables

Anything that can be **counted** is a _discrete_ variable

e.g number of cats in a room, number of tires in a car

Anything that can be **measured** is a _continuous_ variable

e.g. Weight of sugar, time, age, etc

### Check your understanding

#### Numerical or categorical variable?

| Age | Gender | Major      | Units | Housing   | GPA |
|:---:|--------|------------|:-----:|-----------|:---:|
| 18  | Male   | Psychology | 16    | Dorm      | 3.6 |
| 21  | Male   | Nursing    | 15    | Parents   | 3.1 |
| 20  | Female | Business   | 16    | Apartment | 2.8 |

Age, Units, GPA are _numerical_ variable

Gender, Major, Housing are _categorical_ variable

#### Dependent variables

The variable that is altered based on the input variables. Ideally, there is a relationship between the input variable that makes the dependent variable change.

E.g how much sleep you had before you took the test? Studies is a factor that contributes to less sleep.

#### Independent variables

The variable that stands alone and is unaffected by other variables

E.g. What one eats with the age of the person? Both are un-related and hence are independent variables.

## Characteristics of frequency distribution

There are four characteristics of a frequency distribution. They are 

- Modality
- Symmetry
- Central tendency
- Variability

### Modality

The modality is determined by the number of peaks. A _unimodal_ distribution has one peak, a _bimodal_ distribution has two peaks.

![](https://i.imgur.com/1zNmroJ.png)


### Symmetry

A distribution can be _symmetric_ or _asymmetric_.

#### Symmetric distribution

A **symmetric** distribution is a type of distribution where the left side of the distribution mirrors the right side.

![](https://i.imgur.com/RYXKp9O.png)

#### Asymmetric distribution

An **asymmetric** distribution is a type of distribution where the left side and the right side are NOT mirrors of each other.

It can be either _negatively_ skewed or _positively_ skewed.

##### Negatively skewed

In a negatively skewed distribution, the long tail is towards the smaller values

![](https://i.imgur.com/FsFWwGF.png)

##### Positively skewed

In a positively skewed distribution, the long tail is towards the larger values

![](https://i.imgur.com/pKzb2WQ.png)


### Measure of central tendency

A measure of **Central Tendency** is a single value that attempts to describe a set of data by ==identifying the central position within that set of data==. In other words, the Central Tendency computes the "center" around which the data is distributed.

There are three measures of central tendency

- Median
- Mode
- Mean

#### Median

Median is the central value is a set of data.

To find the **median**, we arrange the observations in order from smallest to largest value.

If there is an odd number of observations, the **median** is the middle value. 

If there is an even number of observations, the **median** is the average of the two middle values.

The formula for computing the median is

$$
Median = \space \frac{n + 1}{2}
$$

!!! Note

	Median is less influenced by outliers.

#### Mode

The **mode** of a set of data values is the value that appears most often.

#### Mean

The **mean** (average) of a data set is found by adding all numbers in the data set and then dividing by the number of values in the set

The formula for computing the mean is

$$
Mean \space \mu = \frac{\sum(x)}{n}
$$

#### Measures of central tendency is not sufficient

Let's take an example. 

The following table shows the scores of two players across a series of matches. We need to select one player out of these two. Who would we choose?

!!! Note
	The mean, median and mode are the same.

|  Match | Player A | Player B |
|:------:|:--------:|:--------:|
|    1   |    40    |    40    |
|    2   |    40    |    35    |
|    3   |     7    |    45    |
|    4   |    40    |    52    |
|    5   |     0    |    30    |
|    6   |    90    |    40    |
|    7   |     3    |    29    |
|    8   |    11    |    43    |
|    9   |    120   |    37    |
|   ==Sum==  |    351   |    351   |
|  ==Mean==  |    39    |    39    |
| ==Median== |    40    |    40    |

In cases like these, where we are not able to conclude based on the mean, median and mode, we go with the _measures of dispersion_

### Measures of dispersion

Measures of Dispersion ==describe the data spread== or how far the measurements are from the center.

The measures of dispersion are

- Range
- Variance
- Standard deviation

#### Range

The range is the difference between the maximum value and the minimum value is a data set.

#### Variance

Variance is the difference between each data point and the mean of the data set.

It measures how far a set of numbers are spread out from their average value.

Variance is given by the formula

$$
Variance \space = \frac{\sum(x - \mu)^2}{n}
$$

#### Standard deviation

The Standard Deviation is a measure of how spread out the numbers are.

It is denoted by the letter $\sigma$

A large **standard deviation** indicates that the data points can spread far from the mean and a small **standard deviation** indicates that they are clustered closely around the mean.

The formula for computing the standard deviation (of a population) is 

$$
\sigma = \sqrt \frac{(x - \bar{x})^2}{n}
$$

or standard deviation $\sigma = \sqrt {variance}$

!!! Note "Standard deviation for the sample"

	The formula for computing the standard deviation (of a population) is 

	$$
	\sigma = \sqrt \frac{(x - \bar{x})^2}{n -1}
	$$
	
	where,
	
	$n - 1$ is the degree of freedom.

With the measures of dispersion, let's revisit the previous example and compute the standard deviation

|  Match  | Player A | Player B |
|:-------:|:--------:|:--------:|
|    1    |    40    |    40    |
|    2    |    40    |    35    |
|    3    |     7    |    45    |
|    4    |    40    |    52    |
|    5    |     0    |    30    |
|    6    |    90    |    40    |
|    7    |     3    |    29    |
|    8    |    11    |    43    |
|    9    |    120   |    37    |
|   Sum   |    351   |    351   |
|   Mean  |    39    |    39    |
|  Median |    40    |    40    |
| ==Std Dev== | 41.518   | 7.280    |

We will select player B as the standard deviation is less which means he is more consistent.

## Percentile / Quartile

### Percentile

A **percentile** (or a centile) is a measure used in **statistics** indicating the value below which a given percentage of observations in a group of observations falls. For example, the 20th **percentile** is the value (or score) below which 20% of the observations may be found.

![](https://i.imgur.com/hCt7iwF.png)

Nth percentile states that there are at least N% of values less than or equal to this value and (100-N) values are greater or equal to this value

The formula for finding the number in the N'th percentile is

$$
i = \frac{N}{100}* n
$$

where

$N$ is the percentile we are interested in and
$n$ is the number of values

!!! Note "Key points"

	If i is decimal then round off to next value
	
	If i is an integer then take the average of i and i+1 value

#### Computing percentile in Excel

#### Data

|      |      |      |      |      |      |
|:----:|:----:|:----:|:----:|:----:|:----:|
| 3310 | 3355 | 3450 | 3480 | 3480 | 3490 |
| 3520 | 3540 | 3550 | 3650 | 3730 | 3925 |

#### Solution approach

First, populate the data in excel and then sort it in ascending order

Use the `PERCENTILE.INC` function to get the percentile.

![](https://i.imgur.com/2OaW40I.png)

Use the `PERCENTRANK.INC` function to find the percentile for each value in a range

![](https://i.imgur.com/jasqTb5.png)

### Quartile

Quartile means dividing data % into 4 parts

- Q1 - First Quartile - 25th percentile 
- Q2 - Second Quartile - 50th percentile (Median) 
- Q3 - Third Quartile - 75th percentile

#### Inter Quartile Range (IQR)

IQR is the difference between the third quartile and the first quartile
$IQR = Q3 - Q1$

Let's take the same data and compute the IQR for it

Use the excel function `QUARTILE.INC` to compute the corresponding quartile.

![](https://i.imgur.com/nhKOGfT.png)

## Coefficient of Variation

The coefficient of variation ==shows the extent of variability of data== in a sample about the mean of the population.

The lesser the coefficient of variation, the better.

It is the ratio of the standard deviation to the mean.

The formula for computing the coefficient of variation (CV) is 

$$
CV= \frac{\sigma}{\mu} 
$$

where:

$\sigma$ = standard deviation

$\mu$ = mean​

### Example

Let's take an example and see why the coefficient of variation plays an important part.

#### Data

In an Under 19 World Cup selection squad for 2018, the BCCI needs to select 1 player based on the current performance in 2017 - 2018 Ranji Trophy. There are 2 players with similar stats and the board is not sure whom to select.
Can you help the board members with your analysis?

| Player X | Player Y |
|:--------:|:--------:|
|    40    |    35    |
|    20    |    40    |
|     5    |     7    |
|    20    |    23    |
|    10    |    20    |
|    75    |    26    |
|    100   |    12    |
|    25    |    30    |
|    15    |    27    |
|    15    |    102   |
|    20    |    18    |
|    17    |    17    |
|    11    |    14    |
|     5    |     7    |

#### Solution approach

Let's compute the mean and the standard deviation

|         |  Player X  |   Player Y  |
|:-------:|:----------:|:-----------:|
|         |     40     |      35     |
|         |     20     |      40     |
|         |      5     |      7      |
|         |     20     |      23     |
|         |     10     |      20     |
|         |     75     |      26     |
|         |     100    |      12     |
|         |     25     |      30     |
|         |     15     |      27     |
|         |     15     |     102     |
|         |     20     |      18     |
|         |     17     |      17     |
|         |     11     |      14     |
|         |      5     |      7      |
|   ==Mean==  |     27     |      27     |
| ==Std Dev== | 27.5317998 | 23.70978376 |

The mean is both the same and the standard deviation is almost the same.

How do we decide which player to choose?

Let's compute the coefficient of variation using the formula 

$$
CV= \frac{\sigma}{\mu} 
$$

|         |   Player X  |   Player Y  |
|:-------:|:-----------:|:-----------:|
|         |      40     |      35     |
|         |      20     |      40     |
|         |      5      |      7      |
|         |      20     |      23     |
|         |      10     |      20     |
|         |      75     |      26     |
|         |     100     |      12     |
|         |      25     |      30     |
|         |      15     |      27     |
|         |      15     |     102     |
|         |      20     |      18     |
|         |      17     |      17     |
|         |      11     |      14     |
|         |      5      |      7      |
|   Mean  |      27     |      27     |
| Std Dev |  27.5317998 | 23.70978376 |
|    ==CV==   | 1.019696289 | 0.878140139 |

We see that the CV for the Player Y is much lesser than Player X. Hence, player Y is more consistent and should be selected.

## Correlation and Covariance

What if we need to measure the association between two variables? So far, we have seen only one variable.

We have two measures that will help us determine the association between two variables

- Covariance
- Correlation coefficient

### Covariance

_Covariance_ is a measure of how much two random variables vary together. It's similar to variance, but where variance tells you _how a single variable varies_, covariance tells you _how two variables vary together_.

 here is no meaning of covariance numerical value only sign is useful.

Since covariance is the variance for two variables, the formula is

$$
Cov(X,Y)= \frac{\sum{(X_i - \bar{X})*(Y_i - \bar{Y})}}{n}
$$

$X_i$ = Observation point of variable 

$\bar{X}$ = Mean of all observations (X)

$Y_i$ = Observation point of variable Y

$\bar{Y}$ = Mean of all observations (Y)

$n$ = Number of observations

#### Interpretation

Covariance explains causation between two variables.
Higher the value of covariance, the stronger the relationship between two variables.

Covariance can range from $-\infty \space to +\infty$

### Example

#### Data

Let us take two variables - temperature and the number of customers and try to understand the covariance between these two variables

| Temperature | No of customers |
|:-----------:|:---------------:|
|      97     |        14       |
|      86     |        11       |
|      89     |        9        |
|      84     |        9        |
|      94     |        15       |
|      74     |        7        |

#### Solution approach

Let's do the covariance computation in excel

Go to Data -> Data Analysis and Select "Covariance"

![](https://i.imgur.com/Mt3Bib5.png)

Provide the input range and the output range and click "OK"

![](https://i.imgur.com/9YFf55F.png)

Excel does the computation and shows the covariance between temperature and the number of customers which is $18.72$.

![](https://i.imgur.com/S9LujOr.png)

A positive covariance suggests that these two variables are positively associated. 

But, there is one problem. We don't know to how extent these variables are related or in other words, how strong is their relationship?

This is where Correlation comes into the picture.

### Correlation

Correlation determines the degree or the extent to which the two variables are associated.

The correlation coefficient ranges from $-1 \space to +1$

#### Interpretation

A coefficient greater than $+0.5$ indicates a positive correlation.
A coefficient lesser than $-0.5$ indicates a negative correlation.

#### Formula

$$
r = \frac{Cov(x,y)}{\sigma_x * \sigma_y}
$$

Where

$r$ is the correlation coefficient

$\sigma_x$ is the standard deviation of $x$

$\sigma_y$ is the standard deviation of $y$

#### Solution approach

Let's take the same data and compute the correlation coefficient.

Go to Data -> Data analysis -> Correlation and Click "OK"

![](https://i.imgur.com/El2Hnsg.png)

Provide the input range and the output range and click "OK"

![](https://i.imgur.com/vV3MrAT.png)

We get the correlation coefficient as 0.88

![](https://i.imgur.com/GWZBHvz.png)

This means the variables _temperature_ and _number of customers_ are highly correlated.

Thus correlation provides the extent of correlation between the two variables.

#### Correlation types

**Positive correlation** is a **relationship** between two variables in which both variables move in the same direction. i.e as x increases, y also increases.

E.g. housing prices over time

**Negative correlation** is a **relationship** between two variables in which both variables move in the opposite direction. i.e. as x increases, y decreases.

E.g Health over time

![](https://i.imgur.com/6AafgZg.png)

When there is no correlation between variables, the graph would look like below

![](https://i.imgur.com/Qn6a21d.png)

## Central Limit Theorem (CLT)

The central limit theorem states that if you have a population with mean μ and standard deviation σ and take sufficiently large random samples ($n \ge 30$) from the population, then the distribution of the sample means will be approximately normally distributed.

![](https://i.imgur.com/JOpnLGC.png)

The following three properties hold in the central limit theorem

$$
\mu_{\bar{x}} = \mu
$$

$$
\sigma_{\bar{x}} = \frac{\sigma}{\sqrt n} 
$$

$$
z = \frac{\bar{x} - \mu}{\sigma_{\bar{x}}} = \frac{\bar{x} - \mu}{\frac{\sigma}{\sqrt n}}
$$

## Summary

In this post, we saw what is statistics and how the data is described using descriptive statistics. We have also seen the measures of central tendency, and the measures of variation. 

We touched upon the coefficient of variation and how to measure the association of two variables using covariance and correlation. We finally concluded with Central Limit Theorem which is crucial when we proceed with inferential statistics.


#### Next post

[Inferential statistics](../Inferential_stats_basics)
