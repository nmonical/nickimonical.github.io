## Western States 100 Top Performance Analysis

_**Project description:** In this project I applied web scraping, data cleaning, data visualization, and data analysis skills to identify the top Western States 100 performances of all time._ 

Each year, amidst the scenic backdrop of California's Sierra Nevada Mountains, the world's elite endurance runners converge in Olympic Valley to embark on a grueling 100-mile journey, the Western States Endurance Run. Dating back to 1978, this venerated trail race is a testament to human resilience, pushing athletes to their physical and mental limits. The race commences with a challenging snow-covered ascent, eventually leading runners through scorching canyons where temperatures soar to 100 degrees Fahrenheit. It's a relentless test of endurance, demanding unwavering determination, strategic pacing, and a touch of serendipity.

Since its inception, the WS100 has witnessed remarkable feats of athleticism from both men and women. However, due to a multitude of factors - physiological and otherwise - directly comparing race times across genders can be misleading. This analysis delves into the complexities of gender-based performance in ultramarathon running, seeking to establish a more equitable approach to evaluating and celebrating the most exceptional achievements in this sport. The goal is to create a gender-neutral record book that transcends the boundaries of gender, honoring the pinnacle of human endurance, regardless of biological sex.

The data file was scraped from the WS100 website (https://www.wser.org/results/). The formatting of the results table changed from year to year so the data file needed considerable clean up to be useful. Other things such as missing values and inconsistent data types that needed to be addressed as well.

To perform the analysis, I first explored the data to get a general understanding of how male results compare to female results. In order to develop a gender agnostic record, and ultimately name the greatest performance of all time, I identified the male and female extreme outlier times (i.e. more than 1.5 times the inter-quartile range below the 25th percentile) by gender by year and rank these results according to distance from the 25th percentile. One assumption being made is that the caliber of both the male and female fields are consistent over time. Due to the nature of the entry process to Western States (mostly lottery-based), this should be a fair assumption. The other assumption is that the central tendancies in a given year are a representation of the difficulty of the race (due to snow, heat, course changes, etc.).

<img src="images/wser_chart_1.jpg?raw=true"/>

The results are all within the expected bounds (~14 hours to 30 hours). The bimodal distribution is driven by the personal goal of many to finish within 24 hours (as well as a special award given to those who finish within this time).

<img src="images/wser_chart_2.jpg?raw=true"/>

Female participation increased gradually over the first 20 years of the race, but has held stable at close to 20% of the field since 2000. We would expect the increase in female participation to drive an increase in competition and subsequently improvements in female performance.

<img src="images/wser_chart_3.jpg?raw=true"/>

As expected, winning times for females (and males) have been getting faster over time, though there are fluctuations from year to year, likely due to course conditions as well as the caliber of the front runners in the field. It is interesting to note that in 1995 the top female time was almost the same as the top male time. This was during the period when female participation was still increasing. The small difference between male and female winning times suggests either a week male performance or a strong female performance. We can make this distinction using the gender-agnostic record book.

<img src="images/wser_chart_4.jpg?raw=true"/>

Although the male winning time is consistently faster than the female winning time, in the last 10 years there have been several years when the mean female finishing time was faster than the mean male time. This suggests that in these years there are, relatively speaking, more faster females than faster males.

<img src="images/wser_chart_5.jpg?raw=true"/>

Females are more than 3x as likely to be considered extreme outliers than are males. And the female outliers tend to be even more extreme than the male outliers.

<img src="images/wser_chart_6.jpg?raw=true"/>

This analysis of the Western States Endurance Run (WS100) reveals the top 10 performances of all time, highlighting the remarkable achievements of both male and female athletes. Despite the overall dominance of male runners in the field, females hold a strong presence in the top 10, with Anita Ortiz's 2009 performance securing the top spot. Notably, Ann Trason appears twice in the top 10, though her 1995 run where she almost "beat the boys" is absent. This suggests weakness in the male field that year.

The top 3 performances of all time were achieved by female runners in the 2009 race, demonstrating their exceptional talent and competitive spirit. Interestingly, Jim Walmsley's remarkable 2021 performance, which ranks as the fourth greatest of all time with this methodology, is only his third fastest time, underscoring the notion that evaluating WS100 performances solely based on time may overlook other exceptional achievements.

The WS100 is a grueling test of physical and mental fortitude, and both male and female athletes have demonstrated remarkable resilience and determination in conquering this challenging course. Recognizing and celebrating the top performances, regardless of gender, is crucial to honoring the true spirit of the WS100 and the exceptional athletes who have graced its trails.


