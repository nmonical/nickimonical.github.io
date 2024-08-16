## Western States 100 Top Performance Analysis

_**Project description:** In this project I applied web scraping, data cleaning, data visualization, and data analysis skills to identify the top Western States 100 performances of all time._ 

<img src="images/wser.jpg?raw=true"/>

Each year, amidst the scenic backdrop of California's Sierra Nevada Mountains, the world's elite endurance runners converge in Olympic Valley to embark on a grueling 100-mile journey, the Western States Endurance Run. Dating back to 1978, this venerated trail race is a testament to human resilience, pushing athletes to their physical and mental limits. In some years, the race commences with a challenging snow-covered ascent, and in some years this leads to scorching canyons where temperatures can soar to over 110 degrees Fahrenheit. It's a relentless test of endurance, demanding unwavering determination, strategic pacing, and a lot of serendipity.

Since its inception, the WS100 has witnessed remarkable feats of athleticism from both men and women. However, due to a multitude of factors - physiological and otherwise - directly comparing race times across genders can be misleading. For this project I sought to to establish a more equitable approach to evaluating and celebrating the most exceptional achievements in this sport across the years. The goal was to create a gender-neutral record book that accounted for the range of course conditions that runners are exposed to from year to year.

### Data Collection ###

Data for the analysis was scraped from the WS100 website (https://www.wser.org/results/). Finishing time and gender - the two key variables - were included along with other variables. Before the data could be analyzed, considerable data cleaning was necessary. Finishing time in seconds was also added to the final data set for ease of comparisons. In total there were 10,368 finishers between 1978 and 2023.

### Methodology ###

To perform the analysis, I first explored the data to get a general understanding of how male results compare to female results. In order to develop a gender agnostic record, and ultimately name the greatest performance of all time, I identified the male and female extreme outlier times (i.e. more than 1.5 times the inter-quartile range below the 25th percentile) by gender by year and rank these results according to distance from the 25th percentile. One assumption being made is that the caliber of both the male and female fields are consistent over time. Due to the nature of the entry process to Western States (mostly lottery-based), this should be a fair assumption. The other assumption is that the central tendancies in a given year are a representation of the difficulty of the race (due to snow, heat, course changes, etc.).

### Data Analysis ###

<img src="images/wser_chart_1.jpg?raw=true"/>

First, looking at the finishing time by gender. The results are all within the expected bounds (~14 hours to 30 hours). The bimodal distribution is driven by the personal goal of many to finish within 24 hours (as well as a special award given to those who finish within this time). There are many more males that complete the race than females. 

<img src="images/wser_chart_2.jpg?raw=true"/>

Female participation increased gradually over the first 20 years of the race, but has held stable at close to 20% of the field since 2000. We would expect the increase in female participation to drive an increase in competition and subsequently improvements in female performance.

<img src="images/wser_chart_3.jpg?raw=true"/>

As expected, winning times for females (and males) have been getting faster over time, though there are fluctuations from year to year, likely due to course conditions as well as the caliber of the front runners in the field. It is interesting to note that in 1995 the top female time was almost the same as the top male time. This was during the period when female participation was still growing. The small difference between male and female winning times in this year suggests either a week male performance or a strong female performance. The gender-agnostic record book will help us understand what drove this.

<img src="images/wser_chart_4.jpg?raw=true"/>

Although the male winning time is consistently faster than the female winning time, in the last 10 years there have been several years when the mean female finishing time was faster than the mean male time. This suggests that in these years there are, relatively speaking, more faster females than faster males.

<img src="images/wser_chart_5.jpg?raw=true"/>

Looking at just extreme outliers (those that ran at least 1.5x the inter-quartile range faster than the 25th percentile time by gender), females are more than 3x as likely to be exceptionally fast when compared to their peers. Not only are there more of them but the female outliers tend to be even more extreme than the male outliers.

### Conclusion ###

**Top 10 Performances of All Time**
<img src="images/wser_chart_6.jpg?raw=true"/>

This analysis of the Western States Endurance Run (WS100) reveals the top 10 performances of all time, highlighting the remarkable achievements of both male and female athletes. Despite the overall dominance of male runners in the field, females hold a strong presence in the top 10, with Anita Ortiz's 2009 performance securing the top spot. Notably, Ann Trason appears twice in the top 10, though her 1995 run where she almost "beat the boys" is absent. This suggests that the small difference in times between the male winner and the female winner that year was in fact due to weakness in the male field.

The top 3 performances of all time were achieved by female runners in the 2009 race. This was a notable race as there was a 2 year hiatus due to the cancellation of the 2008 race. Interestingly, Jim Walmsley's remarkable 2021 performance, which ranks as the fourth greatest of all time with this methodology, also followed the cancelled 2020 race.

Perhaps it is physiology, psychology, or other factors driving this trend towards outstanding performances following cancelled races, or it could just be coincidence. What is clear is that since the early editions of the race we have seen an increase in female participation, and in turn increased competition. The fact that 8 of the top 10 performances were run by females demonstrates the competitiveness and tenacity of women in this sport. 

### Further Analysis ###

Moving forward, I am keen to explore alternative methodologies for evaluating the most outstanding performances in ultramarathon history. It would be interesting to develop a bottom-up approach that incorporates factors such as race temperature and the strength of the competition, in contrast to the top-down approach employed in this analysis. Additionally, I am interested in analyzing male and female performances across various races and distances to identify any common trends. By expanding the scope of our investigation, we can gain a more comprehensive understanding of the factors that contribute to exceptional ultramarathon performances.

[See notebook here](https://colab.research.google.com/drive/1AotVQjIV0ryFQbOi6xlTDERW57BgIKLX?usp=sharing)
