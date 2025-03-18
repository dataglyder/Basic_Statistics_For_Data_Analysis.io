## Data Analysts and Statistics
Data Analysts and Scientists adopt some  statistics in their applications to solve problems. I looked at some of the basic ones that are commonly used for data analysis. But before then, let's  talk about table.

## Table
I didn't mean the type your PC is sitting on right now; neither I'm I talking about the type where you set and enjoy your meal, just kidding. Statistical tables are structured ways of presenting data in rows and columns.

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
Measures of central tendency are the mean, meadian and mode - they return the summary of a data with just a single value. They are very easy to calculate with data analytic tools, like spreadsheets(Google sheet and Microsoft Excel Sheet), python and R especially with large data. But in this write up, I'm going to do them the traditional way.
## Mean
It's the average; calculated by adding all the observations and dividing by the total number of observations. So, from the [Cummulative Frequency Distribution](#cummulative-frequency-distribution) table above, $`\ mean = 236/7`$ which is  $`\simeq 34`$.

**Population Mean**

Population mean is the average of all observations being considered in an analysis.Assuming you want to know the average number of blue cars that are within your county; all blue cars within your county represent total population of blue cars. Let's say there are only 6 streets in your county, all blue cars within each streets are counted and the average or mean of these data could be computed as shown below. This type of mean is called **population mean miu/mu/meu** ($`\mu`$) because every blue cars in your county is being counted.

![Total blue cars within the County](https://github.com/dataglyder/Basic_Statistics_For_Data_Analysis.io/blob/main/pop_mean.png)

$`\mu = 216/6 \simeq 36`$ This could be written in statistical symbol as:

$`\mu = \frac{\sum_{i=1}^N x_i}{N}`$

where:


$$\sum$$ = sumation or add

$$^N$$ = total number of observations

$${_i=1}$$ is starting from the first observation

$$x_i$$ = from first observation to the last

***In simple term, sum all obsertaions and divide by its total count.***

**Sample Mean**

Sample mean is a subset of the population that represent the entire population. Taking the mean of the blue cars in your street as shown in [Cummulative Frequency Distribution](#cummulative-frequency-distribution) above is an example of sample mean i.e., Taking a daily sample of blue cars and then the average to represent the entire blue cars that pass on your street daily. The sample mean $`\bar{x}`$ can be represented symbolically as:

$`\bar{x} = \frac{\sum_{i=1}^n x_i}{n}`$

where:


$$\sum$$ = sumation or add

$$^n$$ = total number of observations

$${_i=1}$$ is starting from the first observation

$$x_i$$ = from first observation to the last

Therefore, from table 2, sample mean $`\bar{x} `$ will be:

$`\bar{x} = \frac{30 + 35 + 29 + 34 + 42 + 35 + 31}{7}`$

$`\bar{x} = 34`$

**Note**

**1.** The summary of sample mean is also to add all observations and divide by the count.

**2.** Population mean is represented by meu ($`\mu`$) and it's total count is represented by upper case "N" while sample mean is represented by ($`\bar{x}`$) and its total count is represented by lower case "n".

## Outliers
The down side of using mean is that it can easily be influenced by outliers. outliers are extreme high or low values that are doubted not to be part of the original data due to their extremity. Consider the scenario under the [Cummulative Frequency Distribution](#cummulative-frequency-distribution); if there are days where small number of cars are observed due to for example, weather condition; and people choose to take the bus rather than drive or they choose to work from home, or days where high number of cars are observed due to a party down the street, the average will be low and high in both situations respectively. The two extremes are regarded as outliers. Therefore, a frequency of 2 (due to weather inclement) and 260 (due to a party) are extremes.

## Median
The median is the value that falls at the middle of a distribution after arranging the distribution in an ascending order. These set of values
$`6, 9, 25, 8, 7, 1, 5`$ will have a median of 7 i.e $`1, 5, 6, 7, 8, 9, 25`$ while in $`1, 7, 5, 8, 9, 25`$, the median is 7.5 i.e., arrange the values in ascending order, take the two middle ones, add them together and divide by 2. 

**Note** The benefit of using median is that it is not affected by outliers e.g. 1 and 25 in the set examples are outliers but they do not have any chance to influence the result (median). 
## Mode
The mode is the value that appears most in an array of observations. In $`4, 4, 4, 4, 0, 0, 8, 8, 8, 8, 8, 8, 2, 2, 2, 2, 2, 2, 2, 2, 2`$, the mode is 2-it appears more than any other value in the list of numbers.

## Measures of Despersion
Measures of dispersion indicate the spread of data around the mean. Variance and Standard Deviation are examples of measures of despersion.
## Variance
The variance is the square of the desperse of the data devided by frequency count if dealing with a population or devided by frequency count minus one while dealing with a sample. It could be expressed symbolically as shown below.

**Population Variance**
$`\sigma^2=\frac{\sum_{i=1}^N( x_i-\mu)^2}{N}`$

Let's say I want to know the variance of the weight of harvested tomatoes from my garden (population) for seven days , as in the table below.

![tomato_weight](https://github.com/dataglyder/Basic_Statistics_For_Data_Analysis.io/blob/main/Tomato_table.png)

$`\sigma^2 = \frac{310.96}{7}`$

$`\sigma^2\simeq44`$

**Sample Variance**
$`s^2=\frac{\sum_{i=1}^n( x_i-\bar{x})^2}{n-1}`$

As the manager of my department, assuming I want to know the variance in sales of sugar cookie (sample) for  one week as in the table below.

![cookie_table](https://github.com/dataglyder/Basic_Statistics_For_Data_Analysis.io/blob/main/cookie_sale.png)

$`s^2=\frac{2192.86}{7-1}`$ = $`\frac{2192.86}{6}`$

$`s^2\simeq366`$

***Note*** Be careful with the symbols that are used to represent population variance ($`\sigma`$) and sample variance (s) and also note the changes in the numerator of their equations. In simple term, each tomato weight is approximately 44 square unit away from the mean while each sugar cookie sale is approximately 366 square unit away from the mean. In other to understand better how far these observations are away from the mean, we take the square root of variance; this, is equivalent to standard deviation.

## Standard Deviation
The standard deviation is the square root of variance; $`\sigma=\sqrt{\sigma^2}`$.

**Population Standard Deviation sigma** Could be represented as
$`\sigma =\sqrt{\frac{\sum_{i=1}^N( x_i-\mu)^2}{N}}`$ 

Population standard deviation of tomato weight is:

$`\sigma=\sqrt{44}`$

$`\sigma= 6.6`$

**Sample Standard Deviation s or s.d** Could be represented as: 
$`s=\sqrt {s^2}=\sqrt\frac{\sum_{i=1}^n( x_i-\bar{x})^2}{n-1}`$

Sample Standard deviation of cookie sales is:

$`s=\sqrt{366}`$

$`s=19.1`$

## Example Application of Standard Deviation
Consider the sample mean of 312.86 under sample [variance](#variance) table above, imagine that we have a sale of $`$350`$, that would be about 2 standard deviations to the right from the mean. While a sale of $`$260`$ would be more than 2 standard deviations to the left from the mean.

![sample_Sd and cookie sale](https://github.com/dataglyder/Basic_Statistics_For_Data_Analysis.io/blob/main/applic_sd.png)

## Inferencial Statistics
Still on the [sample variance](#variance) cookie sale, suppose there is a very good day in summer with a lot of parties, and out doors activities that resulted into a sale of $2000 dollars,  or  a 3 days inclement weather that resulted into drop in sale i.e., #50 per day. Of course, these might be regarded as outliers; but should the bumper sale continue throughout the summer and the low sale period extend to all winter. The measures of central tendency and dispersion might not be ideal enough to give us the best insight into the down, peak and low periods within the data; this is where inferencial statistics and the standard normal probability distribution come into play. Inferencial statistics entails making judgement about the whole data population by using just a small portion of the data. 

## The Normal Probability Distribution
Normal probability distribution is a curve that follows a bell shape. Let's say I've upgraded and I now cultivate hectares of tomatoes farm; in my harvesting season, the harvest is low at the beginnig and gradually increase until it reaches the peak of the season and then start declining until the end of the season. The kind of shape gotten from this illustration is the normal distribution curve but with some unique attributes to the statistical normal distribution itself.

**(1)** The total area under the normal distribution is 1.

**(2)** The mean is zero and its standard deviation is 1.

**(3)** The mean and the standard deviation are on the x- axis while the y-axis represents the probability density of the data being analysed.

**(4)** Both ends of the curve extend to infinity; starting from 0 (mean) to the right extend to positive infinity while from 0 (mean) to the left extend to negative infinity. The positivity and negativity  indicate that the standdard deviation lies above or below the mean respectively.
## The Normal Distribution Curve
![Probability Density Curve](https://github.com/dataglyder/Basic_Statistics_For_Data_Analysis.io/blob/main/norm11.png)

## Standardizing Data with the Z-score
To use standard normal distribution to make inference about data, the data should be or assumed to be normally distributed i.e. follow the kind of curve described above, then it could be standardized with a z-score. using the formular:

z=$`\frac{x-\mu}{\sigma}`$ Where:

z= z-score

x= observation

$`\mu`$ = mean

$`\sigma`$=standard deviation

***Note*** that population mean $`\mu`$ and population standard deviation $`\sigma`$ are being used because it is assumed that the whole  population is being considered. In a situation where sample from the population is being used (which is mostly the case), ***standard error*** replaces standard deviation in the z-score. Therefore, z-score for sampled data will be:

z=$`\frac{x-\bar{x}}{\sigma_{\bar{x}}}`$ where $`\sigma_{\bar{x}}`$ is the standrd error.

## Standard Error
Standard error $`\sigma_{\bar{x}}`$ tells us how disperse the sample mean is from the population mean. It replaces standard deviation  while calculating the z-score of a sampled data.
$`\sigma_{\bar{x}}=\frac{\sigma}{\sqrt{n}}`$

$`\sigma`$ = population standard deviation

n = number of sample


Let's assume that my tomatoes harvesting truelly follow a normal distribution with a
$`\mu = 1372.72`$ pounds of tomatoes and $`\sigma= 823.52`$ I can make a number of judgement about the data for example, the probability of getting a certain amount of harvest. But first, the data has to be standardize with the z-score for estimation.
To check the probability of harvesting 2000lb of tomatoes in a day, I can do:
$`z=\frac{x-\mu}{\sigma}`$ 

$`z= \frac{2000-1372.72}{823.52}`$

$`z=0.7617`$ 

Meaning 2000lb harvest is only 0.7617 standard deviation away from mean. The probability of this z-score (0.7617) is then checked on the normal distribution table. 

## How to Check Z-score Probability on a Normal Distribution Table
For a z-score of 0.7617, the first two values fall under z column on the [table](https://z-table.com/)  i.e check for 0.7 row under z, now we are left with 0.0617, check for 0.06 on the top-most row on the table and correspond it to the 0.7 row; e.g., 0.7 row under column 0.06 (Yes! only the 1st 3 values are used) resulting into 0.7617. See [the normal distribution table](https://z-table.com/) for samples.

Therefore, my harvest with z-score 0.7617 has the probability of 0.7764 i.e. 77.64% chance of harvesting 2000lb of tomatoes. This estimate covers all harvest that are less than or equal to 2000lb of harvest.

To check if harvest could be greater than 2000lb:

$`P(harvest>0.7764) = 1 - 0.7764`$ (since the whole normal distribution area is 1)

$`P(harvest>0.7764) = 0.2236 or 22.36%`$

The probability of harvesting 300lb or less  will be
$`z= \frac{300-1372.72}{823.52}`$
$`z = -1.3026`$ This means that getting a harvest of 300lb is 1.3 standard deviation below the mean i.e., to the left. 

Using the normal distribution table, the probability of harvesting 300lb of tomateos with a z-score of -1.3026 is 0.0968 i.e. 9.68% (***Check under the negative z-score table for a negative z-score.***). This estimate indicate the harvest that are less than or equal to 300lb.

To see if harvest could be greater than  300lb:

$`P(harvest>0.0968)= 1- 0.0968=0.9032 or 90.32%

## Estimating from Samples
In a real world scnenario,the whole population might be too large to work with therefore, it's much easier to work with  sample. Any sampling method used must be a representative of the entire population. A minimum of 30 number of samples is needed when z-score is being used for standardization. As long as the sampling method is not biased,  the law of central limit theorem assured us that the sample will be good enough to represent the entire population.
## The Central Limit Theorem
The central limit theorem states that if the number of samples chosen from a population is large enough, the sample means will follow a normal probability distribution irrespective of the shape of the original population. That's a good news! So, the normal distribution, could be used to make inferences about the data. Since the normal distribution is a continuous distribution, a range or interval for estimates could be established with the Confidence interval.

## Confidence Interval and Confidence Level
Confidence interval is a range of values for estimating population parameters and it confidence level might include 80%, 90%, 95%, 99% etc of the normal distribution.The table below shows some examples of confidence intervals and confidence levels.
![Sample Confidence_level_interval](https://github.com/dataglyder/Basic_Statistics_For_Data_Analysis.io/blob/main/con_level_inervl.png) 

Suppose I use 80% confidence interval, this means that I'm 80% confident that the true polpuation mean will lie within the confidence interval estimated, the remaining 20% will not. The 20% error or the number of times that the population mean will not lie within the confidence interval is called alpha $`\alpha`$ or level of significance.
## Level of Significance $`alpha(\alpha)`$
Level of significance $`\alpha`$ is the probability that the true population mean **will not** lie within the confidence interval. For example, a confidence level of 80% will have a significance level of 20% or 0.2 z-score; this will be divided into 2 because the z-score lies above and below the mean i.e. one for the positive end and the other for the negative end. Therefore:

$`0.2  level of significance = z_{\frac{\alpha}{2}} = z_{\frac{0.2}{2}}`$

The closest value to 0.1 under the negative z-score table is in the -1.2 row under column 0.08; $`z_{\frac{0.2}{2}}`$ is therefore 1.28 above the mean and -1.28 below the mean. See the table under [confidence interval and confidence level](#confidence-interval-and-confidence-level) above for some estimated alpha $`\alpha`$.

## How to Calculate Confidence Interval
Assuming I want to determine whether I could achieve a 2000 daily sales of boxes of sugar cookies as the new manager of my store. I might have to use the cookie sales data from my store. While it might be challenging to use the whole population of the cookie sales data, relaying on the law of Central Limit Theorem, I can query the company's database, select at least 30 samples (for z-score standardization), find the mean of the samples, its standard deviation and choose a confidence level. The confidence level is what helps us to determine what the alpha $`(\alpha)`$ will be. 

$`CI=\bar{x}\pm z_{\frac{\alpha}{2}}\sigma_{\bar{x}}`$

So, for a daily cookie sales of 30 number of samples with mean 1864,  standard deviation 18 and a confidence level of 95%, the alpha will be 5%; therefore, the above CI formular can be rewritten as:

$`CI=1864\pm 1.96\sigma_{\bar{x}}`$ 

Don't forget that $`\sigma_{\bar{x}}`$ is the standard error which is standard deviation divided by the square root of number of sample $`\sigma_{\bar{x}}`$= $`\frac{s}{\sqrt{n}}`$

$`\sigma_{\bar{x}} = \frac{18}{\sqrt{30}}`$

$`\sigma_{\bar{x}} = 3.29`$

$`CI = 1864\pm  1.96(3.29)`$ 

CI is within = 1864 - 6.45   and  1864 + 6.45

CI is within = 1857.55  and  1870.45

I am now 95% confidence that the daily sales of boxes of sugar cookie is within intervals 1857.55 and 1870.45; I need to work harder and do things a bit differently to achieve my daily target of 2000 boxes per day. For now, it's not feasible.

Assuming the higher management of my company said, look, you might have drawn from the most recent data we use to sell an average of 1900 boxes of cookies per day. To cornfirm that the true mean of the population is 1900, I will have to conduct hypothesis testing.

## Hypothesis Testing
Hypothesis testing is conducted to varify whether a claim is valid or not. Hypothesis test can be stated in two ways:

**1.** The two tail hypothesis test that is stated with equal to (=) or not equal to ($`\neq`$)

**2** The one tail hypothesis test that is associted with greater than (>), greater than or equal to ($`\geq`$), less than (<), and les than or equal to($`\leq`$) .

**Example Usage of Hypothesis Test**

To varify whether the true mean sales of cookie boxes is 1900, assuming that I selected a cookie sale of 42 number of samples and got a mean of 1872 with a standard deviation of 50 if I choose a 95% confidence interval i.e., alpha is 5% and  conducted my test as follows:

**State my hypothesis:** This is a two tail hypothesis because I'm using "equal to"  and "not equal to" to declare my mean.

**Null Hypothesis $`H_{0}`$**: $`\mu = 1900`$

**Alternate Hypothesis $`H_{1}`$**:  $`\mu\neq 1900`$

**Find the z-score for both means**:

$`z=\frac{\bar{x}-\mu}{\sigma_{\bar{x}}}`$ Remember that $`\sigma_{\bar{x}} = \frac{s}{\sqrt n}`$

$`\sigma_{\bar{x}} = \frac{50}{\sqrt 42}`$

$`\sigma_{\bar{x}}=7.7148`$

Therefore, $`z=\frac{1864-1900}{7.7148}`$ = -3.6294.

## Use Z-score to make Judgement about Estimate
To accept the null hypothsis that the average cookie sale is 1900 boxes per day, the calculated z-score must fall within the region of confidence interval selected which is 95% in this case with $`\alpha`$ of 5% and critical value of -1.96 and 1.96; any z-score value beyond these critical values will be rejected. 
Since -3.6294 falls beyond -1.96, the null hypothsis must be rejected. I can now categorically say that the  mean sales of cookies is not 1900; at least, not for this current period. The data my colleague is referring to might no longer reflect the current shopping attitude or taste of our customers. I have to go with what the customers want for now.

## Use P-value to make Judgement about Estimate
Alternatively, I can check the z-score value on the normal distribution table to get the **p-value**. If the p-val is less than or equal  to `$\alpha`$ I will reject the null hypothesis but if it is greater, I will fail to reject the null hypothesis. In this scenario, the probability of z-score -3.6294 is 0.0001; but because my hypothesis is a two-tail test I will double 0.0001 therefore, my p-value is 0.0002 which is less than my alpha of 0.05. Therefore, I will reject the null hypothesis.  

**Hypothesis Test for two different means**

Let's assume there is a theory that says shoppers buy inorganic bananas because organic bananas are expensive; I doubt it and so quikly become Sherlock Holmes in the malls to investigate the prices of organic and inorganic bananas. I found out that the average price of organic banana per pound across 33 different malls is $0.87 with a standard deviation of 0.23 while that of inorganic is 0.76 with a standard deviation of 0.19. To check whether there is a significant difference between the price of organic and inorganic bananas, I conducted an hypothesis test. 

I stated my hypothesis as:

**Null Hypothesis $`H_{0}`$**: There is no significant difference between the prices of organic and inorganic bananas i.e, $`\mu_{1}-\mu_{2}=0`$

**Alternate Hypothesis $`H_{1}`$**: There is a significant differnce between the prices of organic and inorganic bananas i.e., $`\mu_{1}-\mu_{2}\neq 0`$

Standardizing my observations with z-score I used:

$`z=\frac{(\bar{x}_{1}-\bar{x}_{2})-(\mu_{1}-\mu_{2})}{\sigma_{\bar{x}_{1}- {\bar{x}_{2}}}}`$

$`z=\frac{(\bar{x}_{1}-\bar{x}_{2})-\mu_{1}+\mu_{2}}{\sigma_{\bar{x}_{1}- {\bar{x}_{2}}}}`$

Since $`\mu_{1}-\mu_{2} = 0`$, 

$`z=\frac{\bar{x}_{1}-\bar{x}_{2}}{\sigma_{\bar{x}_{1}-{\bar{x}_{2}}}}`$

But because $`\sigma_{\bar{x}_{1}-{\bar{x}_{2}}}=\sqrt{\frac{\sigma^2_{1}}{n_{1}}+\frac{\sigma^2_{2}}{n_{2}}}`$

$`z=\frac{\bar{x}_{1}-\bar{x}_{2}}{\sqrt{\frac{\sigma^2_{1}}{n_{1}}+\frac{\sigma^2_{2}}{n_{2}}}}`$

Therefore, $`\sigma_{\bar{x}_{1}-{\bar{x}_{2}}}=\sqrt{\frac{(0.23)^2}{33}+\frac{(0.19)^2}{33}}`$ = $`\sqrt{\frac{0.0529}{33}+\frac{0.0361}{33}}`$=$`\sqrt{\frac{0.089}{33}}`$ = $`\sqrt{0.002697}`$= 0.052

Now, $`z=\frac{0.87-0.76}{0.052}`$ =$`\frac{0.11}{0.052}`$=2.115

If I use a confidence interval of 95% meaning my alpha or level of significance will be 0.05. The critical z-score value for alpha ($`\alpha`$) is between -1.96 and 1.96; the banana z-score (2.115) is outside these ranges, therefore, I will reject the null hypothesis and accept the alternate hypothesis. There is a significant difference between the price of organic and inorganic bananas. 

Using P-val to determine my hypothesis, the probability value of z=2.115 from Normal Distribution table is 0.9826; this represent the probability of values less than or equal to z=2.115. To find the probability of values that are greater than z=2.115, subtract 0.9826 from 1 this equals 0.0174. But because there are two tail regions of alpha, 0.0172 is multiplied by 2 which equals 0.0348.Because my p-val(0.0348) is less than alpha of 0.05 I will reject the null hypothesis and accept the alternate hypothesis. There is indeed a significant difference between the price of organic and inorganic bananas.

## The T-Distribution
T-distribution is used when the population standard deviation is unknown and the number of sample (n) is small i.e under 30. The thing is that, the population standard devition is rarely known while analysing big data; we rely on the law of [Central Limit Theorem](#the-central-limit-theorem) to analyse the whole population using the samples that are collected. But i a situation where sample is small i.e., less than 30 to be on the saver side (though, some scholars says 25), the t-distribution is a better choice. When using t-distribution it is important to know the [degree of freedom](https://en.wikipedia.org/wiki/Degrees_of_freedom_(statistics)), choose a [confidence level and alpha($`\alpha`$)](https://datatab.net/tutorial/t-distribution).   
## How to Calculate Confidence Interval Using the T-Distribution
Let's say I want to know my chances of seeing a brown dog walking with its owner on the street of Colorado. If I choose 13 county in Colorado and find the mean of brown dogs walking with thier owner to be 14 (I might have exagerated a bit but seriously, Colorado is very dog friendly) with a standard deviation of 3 and I choose a confidence level of 90%; I can calculate the confidence interval as follows:

confidence interval=$`\bar{x}\pm t_{\frac{\alpha}{2}}s_{\bar{x}}`$ where 

$`\bar{x}\pm t_{\frac{\alpha}{2}}s_{\bar{x}}`$ is called the margine of error

$`\bar{x}=the mean`$ = 14

$`t_{\frac{\alpha}{2}}`$ = the row of the degree of freedom being used under the column of the confidence level or alpha selected. In this case, degree of freedom (df) is n-1 =13-1 =12 and the confident level is 90 or 0.9 and alpha 0.05 (0.10/2). Therefore, $`\alpha=1.782`$ i.e 12 df under confidence level of 90 or alpha 0.05.

$`s_{\bar{x}}`$ = standard error = $`\frac{s}{\sqrt{n}}`$ where

s= standard deviation = 3

n=number of sample = 13

$`s_{\bar{x}} = \frac{3}{\sqrt{13}}`$ = $`\frac{3}{3.606}`$ = 0.83

Therefore, confidence interval=$`14\pm (1.782)(0.83)`$ = $`14\pm \approx2`$ 

the lower level of the confidence interval = 14 - 2 = 12

upper level of the confidence interval = 14 + 2 = 16

This means that the the true population mean of dogs walking with their owners in Colorado is expected to fall within the range of 12 and 16.


## Hypothesis Testing with T-Distribution
Imagine the declaration that people visit their local library more than 4 times in a week. I can conduct hypothesis test to varify this claim. Assuming that I gathered some data and find the average time that people visit their local library per week to be 2 with a standard deviation of 1. Let's say I choose an alpha of 0.05, I can proceed with my varification as follows:

State my hypothesis

**Null Hypothesis $`H_{0}`$**: People visit the library more than 4 times in a week; $`\mu\geq 4`$

**Alternate Hypothesis $`H_{1}`$**: People visit the library less than 4 times in week; $`\mu < 4`$

Calculate the t-test using $`t=\frac{\bar{x}-\mu}{s_{\bar{x}}}`$

since $`s_{\bar{x}}=\frac{s}{\sqrt{n}}`$ =$`\frac{1}{\sqrt{7}}`$=$`\frac{1}{2.646}`$ =0.3779

$`t= \frac{2-4}{0.3779}`$ = $`\frac{-2}{0.3779}`$ =-5.3

My df = n-1 = 7-1=6 under alpha 0.05 = 2.447

Using the left tail of a one tail hypothesis test, the critical t-value 2.447 indicates the region from -2.447 to the right end of the distribution i.e the greater than or equal to($`\geq`$) area as indicated in $`H_{0}`$; this is the do not reject region. My calculated value -5.3 falls below this region i.e., the reject region. Since the calculated value falls within the rejection region, I will reject the null hypothesis and accept the alternative;people visit the library less than 4 times in a week. 

## Hypothesis Testing with T-Distribution and Differences in Two Means
Let's say there is a local Coloradoan that claimed to have seen it all and that he believes there are equal number of black and brown dogs in Colorado. Assume that I call some random dog owners across 19 counties in Colorado and gather the following information to varify his claim.

mean of black dogs = 9 with standard deviation of 4

mean of brown dogs = 12 with standard deviation of 5

There are two ways to go about this.

**1.** I might assume that the variaces of the two dogs are equal. With this assumption, I will have to pool the two variances i.e., average them. Pooled variances  is used when the variances of the two populations are assumed to be equal and therefore averaged using the formular: 

Pooled variance $`S^2_{p}= \frac{(n_{1}-1)s^2_{1}+(n_{2}-1)s^2_{2}}{n_{1}+n_{2}-2}`$ while the pool standard deviation $`S_{p}`$ is $`\sqrt{S^2_{p}}`$

Therefore, to calculate the t-test statistics for equal population variances, the formular is:

$`t=\frac{(\bar{x}_{1}-\bar{x}_{2})-(\mu_{1}-\mu_{2})}{S_{p}\sqrt{\frac{1}{n_{1}}+\frac{1}{n_{2}}}} `$

Now, I can state my hypothesis:

**Null Hypothesis $`H_{0}`$**: Number of black and brown dogs in Colorado are equal: $`\mu_{1} -\mu_{2}=0`$

**Alternate Hypothesis $`H_{1}`$**: Number of brown black and brown dogs in Colorado are not equal: $`\mu_{1} -\mu_{2}\neq0`$

I will calculate the pooled standard deviation $`S_{p}`$ first by taking the square root of the pooled variance.

$`S_{p}`$ =$` \sqrt{\frac{(n_{1}-1)s^2_{1}+(n_{2}-1)s^2_{2}}{n_{1}+n_{2}-2}}`$

$`S_{p} = \sqrt{\frac{(19-1)4^2+(19-1)5^2}{19+19-2}}`$

$`S_{p} = \sqrt{\frac{(18)16+(18)25}{36}}`$

$`S_{p} = \sqrt{\frac{288+450}{36}}`$ = $`\sqrt{\frac{738}{36}}`$ = $`\sqrt{20.5}`$ =4.53

I can now calculate t-statistics $`t =\frac{(\bar{x}_{1}-\bar{x}_{2})-(\mu_{1}-\mu_{2})}{S_{p}\sqrt{\frac{1}{n_{1}}+\frac{1}{n_{2}}}} `$

$`t=\frac{(9-12)-0}{4.53\sqrt{\frac{1}{19}+\frac{1}{19}}} `$ = $`\frac{(-3)-0}{4.53\sqrt{0.05263 + 0.05263}} `$ = $`\frac{-3}{4.53\sqrt{0.10526}} `$ 

$`t =\frac{-3}{1.47} `$ = -2.04

Using alpha $`\alpha`$ 0.05 and with df = 19+19 -2 = 36. **Note** that the degree freedom 36 is not present on the t-distribution table but because the sample "n" is large, I assume it's gradually approaching normal distribution and therefore round up to 40 instead of rounding down to 30. Therefore, my critical t-statistics will be 40 df under two tail $`\alpha`$ 0.05 = 2.021. My calculated t-statistics -2.04 slightly falls outside the range between my critical t-statistics -2.021 and 2.021. I will still reject the null hypothesis and accept the alternate hypothesis.

**2.** The second method to approach t-statistics with two differences in means is to assume that the variances are not equal. So, in this same example of black and brown dogs, I can assume that the variances of the two samples are not equal. With this assumption,the formular below has to be used.

$`t=\frac{(\bar{x}_{1}-\bar{x}_{2})-(\mu_{1}-\mu_{2})}{\sqrt{\frac{s^2_{1}}{n_{1}}+\frac{s^2_{2}}{n_{2}}}} `$ 

The degree of freedom will be computed also using:

$`df=\frac{\left(\frac{s^2_{1}}{n_{1}}+\frac{s^2_{2}}{n_{2}}\right)^2}{\frac{\left(\frac{s^2_{1}}{n_{1}}\right)^2} {n_{1}-1}+ \frac{\left(\frac{s^2_{2}}{n_{2}}\right)^2}{n_{2}-1}}`$

Now, I can state my hypothesis as follows: 

**Null Hypothesis $`H_{0}`$**: Number of black and brown dogs in Colorado are equal: $`\mu_{1} -\mu_{2}=0`$

**Alternate Hypothesis $`H_{1}`$**: Number of brown black and brown dogs in Colorado are not equal: $`\mu_{1} -\mu_{2}\neq0`$

$`t=\frac{(9-12)-0}{\sqrt{\frac{4^2}{19}+\frac{5^2}{19}}}`$=$`\frac{-3}{\sqrt{\frac{16}{19}+\frac{25}{19}}}`$=$`\frac{-3}{\sqrt{0.8421+1.3158}}`$=$`\frac{-3}{1.469}`$ = -2.042

$`df =\frac{\left(\frac{4^2}{19}+\frac{12^2}{19}\right)^2}{\frac{\left(\frac{4^2}{19}\right)^2} {19-1}+ \frac{\left(\frac{12^2}{19}\right)^2}{19-1}}`$

$`df =\frac{\left(2.1579\right)^2}{\frac{\left(0.7091\right)} {18}+ \frac{\left(1.7313)\right)}{18}}`$=34.34

Using $`alpha`$ = 0.05, and rounding my df to 30,my critical t value = 2.042. Since my calculated t-statistics is just right at the lower boundary of the critical t-value, I will fail to reject the null hypothesis.



---
***Please note that all the data that are used in this analysis are assumed data; none of them is real. For further reading, you can check the reference for books that I found helpful.***

***Reference***

[1] Bob Donnelly Jr. and Fatima Abdel-Raouf (2016) "Idiot's Guides Statistics".

[2] Charles Wheelan (2013) "Naked Statistics".

[3] Joseph Schmuller (2016) "Statistical Analysis with Excel"

*** to be continued!***




