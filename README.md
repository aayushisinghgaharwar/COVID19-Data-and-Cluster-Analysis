# COVID19 Data and Cluster Analysis


**Introduction:**

	Since the first case was reported on December 31st, 2019 in Wuhan, China, the novel coronavirus disease (COVID-19) swept the world into a global pandemic. Virtually every country, organization, and person was affected by this virus in some capacity.  As of the end of November 2020, there have been 62.1 million cases, with 39.8 million recovered and 1.45 million deaths, marking that global mortality rate at 2.3%.

In the US alone, there have been over 328,000 cases since January. In response, the White House, private universities, and a coalition of leading research groups have created many datasets that are free to use for the public. Our objective is to conduct an exploratory data analysis and cluster analysis on which areas were most affected by COVID-19. 

Some key questions we want to know is how the virus spread over time, what demographics were most affected, and what geographical clusters exist, if any. Some technologies that will help with our model are PySpark, AWS EMR, Microsoft Excel, Tableau,  and AWS S3. These findings will be significant to figure out how the virus spread and how to prevent it from spreading to more vulnerable communities, as well as which areas may need priority access to the vaccine. In this paper, we will discuss the dataset, the big data visualization techniques, and the models used to answer our key issues. 

Ultimately, the global pandemic is one of the most important issues affecting the world today, and we hope to shed some light on the state of the virus.


**Data Insights:**

	The dataset we used was a collection of datasets compiled by Johns Hopkins University. The data sources include renown research establishments including the WHO, ECDC, CDC, BNO News, and so on.  There are 8 files and 1608 columns, and the largest dataset, which provides geographical and daily information on COVID-19 cases, has over 156,000 rows. 

The dataset spans from January 22nd, 2020, to November 16th, 2020, providing almost 11 months of daily data of confirmed, recovered, and death COVID-19 cases from over 100 countries. A sample of the dataset can be found in the Appendix under Sample Dataset section.

This dataset also includes time-series information of confirmed, death, and recovered on the international and US level, as well as line lists that include characteristics of each case such as age, gender, location, exposure date, and symptoms. 

The time-series data pivot each date as the column and the country on the international data and states on the US level as the row. Some of the variables that we used for our exploratory data analysis were Last Updated, Total Confirmed, Total Recovered, and Total Deaths. 



**Exploratory Data Analysis:**


	To begin our analysis, we started with the daily data to see the timeline of COVID-19. The tables can be seen in the appendix as Table A and Table B. We saw an exponential increase of the number of confirmed cases across the world. At the end of January, there were 10,151 confirmed increases, but by November 16th, there were 54,370,186 cases, with the biggest increase happening between September and October. We saw that in January there were about the same deaths as recoveries, as doctors scrambled to assess all the symptoms and how to manage them. 

However, as doctors had more time and researchers found treatments and medications that mitigate symptoms, we saw recoveries followed a very similar exponential curve to the confirmed cases, while total deaths are increasing much more slowly in comparison. This confirms that many COVID-19 cases do end up with recovery. 

We also looked into the mortality rate, total deaths over total confirmed, to see how that has changed over time. The lowest mortality rate was in January at 2%, and this could be due to the dataset starting on January 22nd, and doctors were unclear if patients were dying from COVID-19 or another illness. The highest mortality rate was at 7% in April, which was when COVID-19 cases started to exponentially increase all across the world. 

Now, mortality rate is at 2.4% and is slowly decreasing as doctors are able to successfully treat patients, and with a new vaccine on the horizon, hopefully it will decrease even further. 

