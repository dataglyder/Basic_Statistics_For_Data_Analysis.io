## Data Analysts and Statistics
Data Analysts and Scientists adopt some  statistics in their applications to solve problems. I looked at some of the basic ones that are commonly used for data analysis. But before then, let's,  talk about table.

## Table
I didn't mean the type your PC is sitting on right now; neither I'm I talking about the type where you set and enjoy your meal! Just kidding. Statistical tables are structured ways of presenting data in rows and columns.

**A Table with Rows and Columns**


![A Sample Table with Rows and Columns](https://github.com/dataglyder/Basic_Statistics_For_Data_Analysis.io/blob/main/row_col.png)


How the data is organized in the table can give the table a slightly unique name such as: frequency distribution table, cummulative frequncy distribution table, contingency table, etc. 
### Frequency Distribution Table
This displays the observed data and the total time it occured. Imagine that you want to know how many blue cars pass on your street daily, so, you decided to take daily data of blue cars that pass on your street for one week. Below is a simple frequency table summarising a likely outcome.

![Frequency Distribution Table](https://github.com/dataglyder/Basic_Statistics_For_Data_Analysis.io/blob/main/freq_table.png)

### Cummulative Frequency Distribution
Frequency distribution table becomes cummulative distribution table by adding the frequencies in a subsequent order as shown below.

![Cummulative Frequency Table](https://github.com/dataglyder/Basic_Statistics_For_Data_Analysis.io/blob/main/cum_freq.png)

### Contingency Table
Contigency tables are used to represent variables that are more than one. Consider a dealer who gathers data about his car sales by color so as to determine what quantity to keep in stock by color. The contingency table below might represent data collected. 

![Contingency Table](https://github.com/dataglyder/Basic_Statistics_For_Data_Analysis.io/blob/main/contingen_table.png)

***Enough about table! Now, let's move on to something else.***

## Descriptive Statistics
Descriptive statistics involves the use of ***measures of central tendency*** and ***measures of dispersion*** to gain knowledge and also probably make decisions about data.
## Measures of Central Tendency
Measures of central tendency are the mean, meadian and mode - they return a single value as the center point of the data (Bob and Fatma 2016, p.50)[1]. They are very easy to calculate with data analytic tools, like spreadsheets(Google sheet and Microsoft Excel Sheet), python and R especially with large data. But in this write up, I'm going to do them the traditional way.
### Mean
It's the average; calculated by adding all the observations and dividing by the total number of observations. So, from the [Cummulative Frequency Distribution](#cummulative-frequency-distribution) table above, $`\ mean = 236/7`$ which is  $`\simeq 34`$.

**Population Mean**

Population mean is the average of all observations being considered in an analysis.Assuming you want to know the total number of blue cars that are within your county instead of just your street; all blue cars within your county represent total population of blue cars. Let's say there are only 6 streets in your county, all blue cars within each streets are counted and the average or mean of these data could be computed as shown below. This type of mean is called **population mean miu/mu/meu** ($`\mu`$).

![Total blue cars within the County](https://github.com/dataglyder/Basic_Statistics_For_Data_Analysis.io/blob/main/pop_mean.png)

$`\mu = 216/6 \simeq 36`$ This could be statistically represented as:

$`\mu = \frac{\sum_{i=1}^N x_i}{N}`$

where:


$$\sum$$ = sumation or add

$$^N$$ = total number of observations

$${_i=1}$$ is starting from the first observation

$$x_i$$ = from first observation to the last

***In simple term, sum all obsertaions and divide by its total count.***

**Sample Mean**

Sample mean is a subset of the population that represent the entire population. Taking the mean of the blue cars in your street as shown in [frequency distribution table]() above is an example of sample mean i.e., Taking a daily sample of blue cars and then the average to represent the entire blue cars that pass on your street daily. The sample mean \bar{x} can be represented mathematically as:

$`\bar{x} = \frac{\sum_{i=1}^n x_i}{n}`$

where:


$$\sum$$ = sumation or add

$$^n$$ = total number of observations

$${_i=1}$$ is starting from the first observation

$$x_i$$ = from first observation to the last

Therefore, from table 2, sample mean $`\bar{x} `$ will be:

$$\bar{x} = \frac{30 + 35 + 29 + 34 + 42 + 35 + 31}{7}$$
$$\bar{x} = 34$$

**Note**

**1.** The summary of sample mean is also to add all observations and divide by the count.

**2.** Population mean is represented by meu ($`\mu`$) and it's total count is represented by upper case "N" while sample mean is represented by ($`\bar{x}`$) and its total count is represented by lower case "n".

## Outliers
The down side of using mean is that it can easily be influenced by outliers. outliers are extreme high or low values that are doubted not to be part of the original data due to their extremity. Consider the scenario under the [frequency distribution table](); if there are days where small number of cars are observed due to for example, weather condition; and people choose to take the bus rather than drive or they choose to work from home, or days where high number of cars are observed due to a party down the street, the average will be low and high in both situations respectively. The two extremes are regarded as outliers. Therefore, a frequency of 2 (due to weather inclement) and 260 (due to a party) are extremes.

## Median
The median is the value that falls at the middle of a distribution after arranging the distribution in an ascending order. These set of values
$`6, 9, 25, 8, 7, 1, 5`$ will have a median of 7 i.e $`1, 5, 6, 7, 8, 9, 25`$ while in $`1, 7, 5, 8, 9, 25`$, the median is 7.5 i.e., arrange the values in ascending order, take the two middle ones, add them together and divide by 2. 

**Note** The benefit of using median is that it is not affected by outliers e.g. 1 and 25 in the set examples. 
## Mode
The mode is the value that appears most in an array of observations. In $`4, 4, 4, 4, 0, 0, 8, 8, 8, 8, 8, 8, 2, 2, 2, 2, 2, 2, 2, 2, 2`$, the mode is 2.

## Measures of Despersion
Measures of dispersion indicate the spread of data around the mean. Variance, Standard Deviation and Range are examples of measures of despersion.
### Variance
The variance is the square of the desperse of the data devided by frequency count if dealing with a population or devided by frequency count minus one while dealing with a sample. It could be expressed mathematically as shown below.

**Population Variance**
$`\sigma^2=\frac{\sum_{i=1}^N( x_i-\mu)^2}{N}`$

Let's say I want to know the variance of the weight of harvested tomatoes from my garden (population) for seven days , as in the table below.

![tomato_weight]()

$`\sigma^2 = \frac{310.96}{7}`$

$`\sigma^2\simeq44`$

**Sample Variance**
$`s^2=\frac{\sum_{i=1}^n( x_i-\bar{x})^2}{n-1}`$

As the manager of my department, assuming I want to know the variance in sales of sugar cookie (sample) for  one week as in the table below.

![cookie_table]()

$`s^2=\frac{2192.86}{6}`$

$`s^2\simeq366`$

***Note*** In simple term, each tomato weight is approximately 44 square unit away from the mean while each sugar cookie sale is approximately 366 square unit away from the mean. In other to understand better how far these observations are away from the mean, we take the square root of variance; this, is equivalent to standard deviation.

## Standard Deviation
The standard deviation is the square root of variance.
$`\sigma=\sqrt\sigma^2=\sqrt\frac{\sum_{i=1}^N( x_i-\mu)^2}{N}`$ for population standard deviation and $`s=\sqrt s^2=\sqrt\frac{\sum_{i=1}^n( x_i-\bar{x})^2}{n-1}`$ for sample standard deviation

Population standard deviation of tomato weight is:

$`\sigma=\sqrt44`$

$`\sigma= 6.6`$

Sample Standard deviation of cookie sales is:

$`s=\sqrt366`$

$`s=19.1`$

## Application of Standard Deviation
Consider our ![cookie sale table](), imagine that we have a sale of $`$400`$, that would be about 5 standard deviation (4.6) to the right from the mean. While a sale of $`$250`$ would be approximately 3 standard deviation (3.3) from the mean.
##[Sd and cookie sale]()
Now, suppose there is a very good day in summer with a lot of parties, and out doors activities and there is a sale of $2000 dollars,  or 3 days inclement weather that resulted into drop in sale i.e., #50 per day. Of course, these might be regarded as outliers; but suppose the bumper sale continue throughout the summer while the low sale period extend to all winter. The measures of central tendency and dispersion might not be ideal enought to give us the best insight into the down, peak and low period within the data; this is where inferencial statistics and the standard normal probability distribution come into play.

### Range
Range is the difference between the highest and the lowest observation in an array of data. The range of $`1, 5, 6, 7, 8, 9, 25`$ is 24. i.e., $`25-1`$

## The Normal Probability Distribution
Normal probability distribution is a curve that follows a bell shape. Let's assume our [tomates harvesting] is from hectares of  land and was at the beginnig of the harvesting period  and gradually climb until it reaches the peak of the season and then start declining until the end of the season. The kind of shape gotten from this illustration is the normal distribution curve but with some unique attributes to the statistical normal distribution itself.

**(1)** The total area under the normal distribution is 1

**(2)** The mean is zero and it has standard deviation is 1.

**(3)** The mean and the standard deviation are on the x- axis while the y-axis represents the probability density of the data being analysed.

**(4)** Both ends of the curve extend to infinity

**(5)** Starting from 0 (mean) to the right extend to positive infinity while from 0 (mean) to the left extend to negative infinity; the positivity and negativity only indicates that the standdard deviation lies above or below the mean respectively.
![Probability Density Curve]()

## Standardizing Data with the Z-score
In other to use standard normal distribution to make inference about our data, the data must first be standardized with a z-score. using the formular:

z=$`\frac{x-\mu}{\sigma}`$ Where:

z= z-score

x= observation

$`\mu`$ = mean

$`\sigma`$=standard deviation
***Note*** that population mean $`\mu`$ and population standard deviation $`\sigma`$ are being used because it is assumed that the whole  population is being considered. In a situation where sample from the population is being used (which is mostly the case), ***standard error*** replaces standard deviation in the z-score. Therefore, z-score for sampled data will be:

z=$`\frac{x-\bar{x}}{\sigma_{\bar{x}}}`$ where $`\sigma_{\bar{x}}`$ is the standrd error.

### Standard Error
$`\sigma_{\bar{x}}=\frac{\sigma}{\sqrt{n}}`$

$`\sigma`$ = population standard deviation

n = number of sample


Let's say my tomatoes harvesting truelly follow a normal distribution and several pounds were harvested daily as shown in the table below; resulting in the normal distribution that follows.

![tom_table]()

$`\mu = 1372.72`$

$`\sigma= 823.52`$

![Distribution curve]()

Standard normal distribution has a mean of 0,therefore, the data has to be standardize with the z-score for estimation.
To check the probability of harvesting 2000lb of tomatoes in a day, we can do:
$`z=\frac{x-\mu}{\sigma}`$ 

$`z= $`\frac{2000-1372.72}{823.52}`$

$`z=0.7617`$ Meaning 2000lb harvest is only 0.7617 standard deviation away from mean.
Now, ![check z-score pro]() ![the normal distribution table](https://z-table.com/) could be used to find the probability of harvesting 2000lb of tomatoes. 


z-score 0.7617 has a probability of 0.7764 i.e. 77.64% chance of harvesting 2000lb of tomatoes per day.


The probability of harvesting 300lb will be
$`z= \frac{300-1372.72}{823.52}`$
$`z = -1.3026`$ This means getting a harvest of 300lb is 1.3 standard deviation below the mean. 

Using the normal distribution table, the probability of harvesting 300lb of tomateos is 0.0968 i.e. 9.68%

These values estimated are range of values that extends to the tail of the distribution meaning that harvest could be 2000lb or less, 300lb pounds or less. 

To see if harvest could be greater than 2000lb or 300lb:

$`P(harvest>0.7764) = 1 - 0.7764`$ (since the whole normal distribution area is 1)

$`P(harvest>0.7764)=0.2236 06 22.36%`$

$`$`P(harvest>0.0968)= 1- 0.0968=0.9032 or 90.32%

## Estimating from Samples
In a real world scnenario,the whole population might be too large to work with therefore, it's much easier to work with  sample. Any sampling method used must be a representative of the entire population. A minimum 30 number of samples is needed if z-score is  adopted but if number of sample is less than 30, T-distribution is more desirable. Whichever sampling method is adopted, the law of central limit theorem assured us that the sample is good enough to represent the entire population.
## The central Limit Theorem
The central limit theorem states that if the number of samples chosen from a population is large enough, the sample means will follow a normal probability distribution irrespective of the shape of the original population. That's a good news! So, the normal distribution, could be used to make inferences about the data. Since the normal distribution is a continuous distribution, a range or interval for estimates could be established with the Confidence interval.

## Confidence Interval and Confidence level
Confidence interval is a range of values for estimating population parameters and it confidence level might include 80%, 90%, 95%, 99% etc of the normal distribution.![Sample Confidence_level_interval]() Suppose I use 80% confidence interval, this means that I'm 80% confident that the true polpuation mean will lie within the confidence interval estimated, the remaining 20% will not. The 20% error or the number of times that the population mean will not lie within the confidence interval is called alpha $`\alpha`$ or level of significance.
## Level of Significance $`alpha(\alpha)`$
Level of significance $`\alpha`$ is the probability that the true population mean **will not** lie within the confidence interval. For example, a confidence level of 80% will have a significance level of 20% or 0.2 z-score; this will be divided into 2 because the z-score lies above and below the mean i.e. one for the positive end and the other for the negative end. Therefore:

$`0.2  level of significance = z_{\frac{\alpha}{2}} = z_{\frac{0.2}{2}}`$

The closest value to 0.1 under the negative z-score table is in the -1.2 row under column 0.08; $`z_{\frac{0.2}{2}}`$ is 1.28 above the mean and -1.28 below the mean.

## How to Calculate Confidence Interval
Assuming I want to determiine whether I could achieve a 2000 daily sales of boxes of sugar cookies as the new manager of my store. I might have to use the cookie sales data from my store. While it might be challenging to use the whole population of the cookie sales data, relaying on the law of Central Limit Theorem, I can query the company's database, select at least 30 samples (using z-score), find the mean of the samples, its standard deviation and choose a confidence level. The confidence level is what helps us to determine what the alpha $`(\alpha)`$ will be. 

$`CI=\bar{x}\pm z_{\frac{\alpha}{2}}\sigma_{\bar{x}}`$

So, for a daily cookie sales of 30 number of samples with mean 1864,  standard deviation 18 and a confidence level of 95%, the alpha will be 5%; therefore, the above CI formular can be rewritten as:

$`CI=1864\pm 1.96\sigma_{\bar{x}}`$ 

Don't forget that $`\sigma_{\bar{x}}`$ is the standard error which is standard deviation divided by the square root of number of sample $`\sigma_{\bar{x}}`$= $`\frac{s}{\sqrt{n}}`$ I'm using sample standard deviation

$`\sigma_{\bar{x}} = \frac{18}{\sqrt{30}}`$

$`\sigma_{\bar{x}} = 3.29`$

$`CI = 1864\pm  1.96(3.29)`$ 

CI is within = 1864 - 6.45   and  1864 + 6.45

CI is within = 1857.55  and  1870.45

I am now 95% confidence that the daily sales of boxes of sugar cookie is within intervals 1857.55 and 1870.45; I need to work harder and do things a bit differently to achieve my daily target of 2000 boxes per day. For now, it's not feasible.
Assuming the higher management of my company said, look, you might have drawn from the most recent data; we use to sell an average of 1900 boxes of cookies per day. To cornfirm that the true mean of the population is 1900, I will have to conduct hypothesis testing.

## Hypothesis Testing
Hypothesis testing is conducted to varify the validity of a claim about a population based on a single sample [cite]. To varify whether there is a significant difference between 1864 and 1900  sales of cookie boxes, I choose a 95% confidence interval i.e., alpha is 5% and  conducted my test as follows:

**State my hypothesis**

**Null Hypothesis $`H_{0}`$**: $`\mu = 1900`$

**Alternate Hypothesis $`H_{1}`$**:  $`\mu\neq 1900`$

**Find the z-score for both means**:

$`z=\frac{\bar{x}-\mu}{\sigma_{\bar{x}}}`$ Remember that $`\sigma_{\bar{x}} = \frac{s}{\sqrt n}`$
$`\sigma_{\bar{x}} = \frac{18}{\sqrt 30}
$`\sigma_{\bar{x}}=3.286

Therefore, $`z=\frac{1864-1900}{3.286}`$ = -10.956 as shown in the distribution below.
![Distribution]()

Since the calculated z-score value falls outside the no-rejection area, I have to reject the null hypothesis $`H_{0}`$. Possibly, the data my colleague is talking about is an outdated data that does not reflect the current shopping attitude or taste of our customers. I have to go with what the customers want for now.

Let's assume that I've worked realy hard to meet my target sales of 2000 boxes per day, but there is a competitive company that is selling an average of 2100 boxes per day and I'm curious to know if there is any significant difference between their sales and ours? To varify this, I conducted another hypothesis test.



**Null Hypothesis $`H_{0}`$**: There is no significant difference between 1864 and 1900 boxes of cookies i., $`\mu `$

**Alternate Hypothesis $`H_{1}`$**: There is a significant differnce between 1864 and 1900 boxes of cookies i.e., $`\mu`$
















 ## How to Check Z-score Probability on a Normal Distribution Table
For a z-score of 0.7617, the first two values fall under z column on the table i.e check for 0.7 row under z, now we are left with 0.0617 now, check for 0.06 column on the top-most row on the table; the final value is  0.7 row under column 0.06 (Yes! only the 1st 3 values are used). 


---
***For further reading, you can check the reference for books that I found helpful.***

***Reference***

[1] Donnelly B. Jr., Abdel-Raouf F. (2016) "Idiot's Guides Statistics".

***To be edited and continued!***




