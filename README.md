## Data Analysts and Statistics
Data Analysts and Scientists adopt some  statistics in their applications to solve problems. I looked at some of the basic ones that are commonly used for data analysis. But before then, let's,  talk about table first

## Table
I didn't mean the type your PC is sitting on right now; neither I'm I talking about the type where you set and enjoy your meal! Just kidding. Statistical tables are structured ways of presenting data in rows and columns.

**A Table with Rows and Columns**


![A Sample Table in Rows and Columns](https://github.com/dataglyder/Basic_Statistics_For_Data_Analysis.io/blob/main/Screenshot%202025-02-09%20101732.png)


How the data is organized in the table can give the table a slightly unique name such as: distribution frequency table, contingency table, cummulative frequncy distribution table etc. 
### Frequncy Distribution Table
This displays the observed data and the total time it occured. Imagine that you want to know how mny blue cars pass on your street daily, so, you decided to take daily data of blue cars that pass on your street for one week. Below is a simple frequency table summarising a likely outcome.

***Table 1***
![Table 1 Frequency Distribution Table](https://github.com/dataglyder/Basic_Statistics_For_Data_Analysis.io/blob/main/freq_table.png)

### Cummulative Frequency Distribution
Frequency distribtion table becomes cummulative distribution table by adding the frequencies in a subsequent order as shown below.

***Table 2***
![Table 2 Cummulative Frequency Table](https://github.com/dataglyder/Basic_Statistics_For_Data_Analysis.io/blob/main/cum_freq.png)
### Contingency Table
Contigency tables are used to represent variables that are more than one. Consider a deler who gathers data about his car sales by color so that he could know what quantity to keep in stock by color. The contingency table below might represent data collected. 

***Table 3***
![Table 3 Contingency Table](https://github.com/dataglyder/Basic_Statistics_For_Data_Analysis.io/blob/main/contingen_table.png)

*** Enough about table! You can learn more on [tables]()
## Descriptive Statistics
Descriptive statistics involves the use of ***measures of central tendency*** and ***measures of dispersion*** to gain knowledge and also probably make decisions about data.
## Measures of Central Tendency
Measures of central tendency are the mean, meadian and mode - they return a single value as the center point of the data [1]. They are very easy to calculate with data analytic tools, like spreadsheets(Google sheet and Microsoft Excel Sheet), python and R especially with large data. 
### Mean
It's the average; calculated by adding all the observations and dividing by the total number of observations. So, from table 2 above, $`\ mean = 236/7`$ which is  $`\simeq 34`$.

**Population Mean**

Assuming you want to know the total number of blue cars that are within your county instead of just your street, all blue cars within your county represent total population of blue cars. It might be challenging to count all these cars at onces but data could be collected from six strategic street within your county, and the average or mean of these data could be computed. This type of mean is called ***population mean miu/mu/meu** ($`\mu`$). Table 4 below represents sample data that might be collected.

***Table 4***
![Total blue cars within the County](https://github.com/dataglyder/Basic_Statistics_For_Data_Analysis.io/blob/main/pop_mean.png)

$`\mu = 216/6 \simeq 36`$ This could be statistically represented as:

$$\mu = \frac{\sum_{i=1}^N x_i}{N}$$

where:


$$\sum$$ = sumation or add

$$^N$$ = total number of observations

$${_i=1}$$ is starting from the first observation

$$x_i$$ = from first observation to the last

***In simple term, sum all obsertaions and divide by its total count.***

**Sample Mean**

Taking the mean of the blue cars in just your street as shown in frequency [distribution]() above instead of the whole county is an example of sample mean. The sample mean \bar{x} can be represented mathematically as:

$$\bar{x} = \frac{\sum_{i=1}^n x_i}{n}$$

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
The down side of using mean is that it can easily be influenced by outliers. outliers are extreme high or low values that are doubted not to be part of the original data due to their extremity. Imagine the scenario under the [frequency distribution table](); if there are days where small number of cars are observed due to for example, weather condition; and people choose to take the bus rather than drive or work from home, or days where high number of cars are observed due to a party down the street, the average will be low and high in both situations respectively. The two extremes are regarded as outliers. Consider table 2 above, a frequency of 2 (due to weather inclement) and 1,260 (due to party) are extremes.

## Median
The median is the value that falls at the middle of a distribution after arranging the distibution in an ascending order. These set of values
$`6, 9, 25, 8, 7, 1, 5`$ will have a median of 7 i.e $`1, 5, 6, 7, 8, 9, 25`$ and in $`1,7 5, 8, 9, 25`$, the median is 7.5 i.e., arrange the values in ascending order, take the two middle ones, add them together and divide by 2. 

**Note** The benefit of using median is that it is not affected by outliers (1 and 25) in the set examples. 
## Mode
The mode is the value that appears most in an array of observations. In $`4, 4, 4, 4, 0, 0, 8, 8, 8, 8, 8, 8, 2, 2, 2, 2, 2, 2, 2, 2, 2`$, the mode is 2.

## Measures of Despersion
Measures of dispersion indicate the spread of data around the mean. Variance, Standard Deviation and Range are examples of measures of despersion.
### Variance
The variance is the square of the desperse of the data devided by frequency count if dealing with a population or devided by frequency count minus one while dealing with a sample. It could be expressed mathematically as shown below.

**Population Variance**
$$\sigma=\frac{\sum_{i=1}^N( x_i-\bar{x})^2}{N}$$

**Sample Variance**
$$s=\frac{\sum_{i=1}^n( x_i-\bar{x})^2}{n-1}$$

Let's say the chairman board of agriculture in Ohio state wants to know the quantity of tomatoes that are consumed in the city of Painesville per month and so, he ordered all grocery stores to turn in their data of tomatoe sales. Assuming there are 12 grocery stores in Painesville, as in the table below, the average sale could be considered as the total population of tomatoes.
![tomates pop]()
$`\sum_{i=1}^N( x_i-\bar{x})^2= 178998.9`$

## Standard Deviation

### Range
Range is the difference between the highest and the lowest observation in an array of data. The range of $`1, 5, 6, 7, 8, 9, 25`$ is 24. i.e., `$25-1`$

***To be edited and continued!***




