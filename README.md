## Data Analysts and Statistics
Data Analysts and Scientists adopt some  statistics in their applications to solve problems. I looked at some of the basic ones that are usually used for data analysis. 

## Table
I didn't mean the type your PC is sitting on right now; neither I'm I talking about the type where you set and enjoy your meal! Just kidding. Statistical tables are structured ways of presenting data in rows and columns.

**A Table with Rows and Columns**

<span
style="display:block; text-align:center">
![A Sample Table in Rows and Columns](https://github.com/dataglyder/Basic_Statistics_For_Data_Analysis.io/blob/main/Screenshot%202025-02-09%20101732.png)</span>


How the data is organized in the table can give the table a slightly unique name such as: distribution frequency table, contingency table, cummulative frequncy distribution table etc. 
### Frequncy Distribution Table
This displays the observed data and the total time it occured. Imagine that you want to know how mny blue cars pass on your street daily, so, you decided to take daily data of blue cars that pass on your street for one week. Below is a simple frequency table summarising a likely outcome.

![Table 1 Frequency Distribution Table](https://github.com/dataglyder/Basic_Statistics_For_Data_Analysis.io/blob/main/freq_table.png)

### Cummulative Frequency Distribution
Frequency distribtion table becomes cummulative distribution table by adding the frequencies in a subsequent order as shown below.
![Table 2 Cummulative Frequency Table]()
### Contingency Table
Contigency tables are used to represent variables that are more than one. Consider a deler who gathers data about his car sales by color so that he could know what quantity to keep in stock by color. The contingency table below might represent data collected. 
![Table 3 Contingency Table]()
## Descriptive Statistics
Descriptive statistics involves the use of ***measures of central tendency*** and ***measures of dispersion*** to gain knowledge and also probably make decisions about data.
## Measures of Central Tendency
Measures of central tendency are the mean, meadian and mode. They are very easy to calculate with data analytic tools, like spreadsheets(Google sheet and Microsoft Excel Sheet), python and R. 
### Mean
It's the average; calculated by adding all the observations and dividing by the total number of observations. So, from table 2 above, $`\ mean = 236/7`$ which is  $`\simeq 34`$.

**Population Mean**
Assuming you want to know the total number of blues cars that are within your county instead of just your street, all blue cars within your county represent total population of blue cars. It might be challenging to count all these cars at onces but data could be collected from six strategic street within your county, and the average or mean of these data could be computed. This type of mean is called ***population mean miu/mu/meu** ($`\mu`$). Table 4 below represents sample data that might be collected
![Total blue cars within the County]()

$`\mu = 216/6 \simeq 36`$ This could be statistically represented as:

$$\mu = \left( \sum_{i=1}^N x_i \right)/N$$

where:


$$\sum$$ = sumation or add

$$^n$$ = total number of observations

$${_i=1}$$ is starting from the first observation

$$x_i$$ = from first observation to the last

***In simple term, sum all obsertaions and divide by its total count.***

**Sample Mean**



. Take for instance, if I want to know the total number of cars that pass my street in a day, I can observe this for one week and then take the average. The down side to this method is that if there are days where small number of cars are observed due to for example, weather condition, and people choose to take the bus rather than drive or work from home, or days where high number of cars are observed due to a party down my street, the average will be low and high in both situations respectively. The two extreams are regarded as outliers. Consider the table, if between 65 to 85 cars will pass through the street par day, the couunt of 2 and 1,260 are the extreams.
![Mean_table]()

**Use the formular beloow to calculate mean**
$$\left( \sum_{k=1}^n a_k b_k\right)$$

***To be edited and continued!***



