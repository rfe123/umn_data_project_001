# Group 6 - Project 1

## Data Cleaning
	To understand our data, some quick visualizations were run. Sophie Geister-Jones created visuals of the dataset based on gender, age, blood pressure, and sleep disorder diagnosis. We noticed that there seemed to be a larger amount of study participants that have hypertensive blood pressure than would be expected.
	Bob Erickson did the majority of cleaning the data when we were all first exploring it. He split the blood pressure into two columns that were labeled as Systolic and Diastolic. That allowed Sophie Geister-Jones to create a qualitative column for blood pressure that labeled the data as “low,” “normal,” “elevated,” or “hypertensive.” Additionally, Erickson also cleaned up the Sleep Disorder column by replacing “NaN” values with “No Diagnosis”.

## Analysis Questions
	The Sleep Health and Lifestyle Dataset uploaded on Kaggle.com by Laksika Tharmalingam (2023) contained data on 374 individuals’ gender, age, sleep duration and quality, stress level, physical activity level, blood pressure, and BMI standing. After examining the raw data, we had three questions we wished to investigate: (1) How does sleep relate individually to level of fitness during the day? (2) How does sleep relate to general stress levels? (3) Does gender and age affect the variables in a statistically significant way?
  We hypothesized that the best way to search for any potential relationships was to analyze the relationship between sleep and fitness, sleep and stress, and stress and fitness and to see if any one relationship had a stronger correlation than others.

### Sleep and Physical Activity
We examined the relationship between sleep and fitness level. Sleep duration is measured in hours and physical activity level is the minutes per day a person engages in physical activity. There are a few potential outliers within the data set that could be skewing results as shown in a box and whiskers plot created between the sleep duration and phydical activity level.

A scatter plot shows a slightly positive correlation. These graphs show that for the extreme physical activity levels there are wide ranges of sleep duration. In general we noted higher physical activity level correlates with sleep duration.

### Sleep and Stress Levels
There's a negative correlation between sleep duration and stress level:
• Having longer sleep durations might be associated with lower stress levels, indicating the potential importance of sufficient sleep in managing stress.
• Similarly, shorter sleep durations might be associated with higher stress levels, suggesting that inadequate sleep could contribute to increased stress levels.

Stress Level Frequencies :
• Male are facing more stress levels compared to female's.
• Female stress levels are very low based on the available data.

### Relationship between Fitness & Stress
There is a weak correlation for how daily steps alone affects physical fitness level:
- Male Data:R-squared: 0.17
Explanation: The number means that the daily steps can explain about 17% of why stress levels vary among males, suggesting a weak relationship
- Female Data:R-squared: 0.34
Explanation: For females, the daily steps explain around 34% of the variance in stress levels. This relationship is more noticeable compared to the males, but still not a strong correlation.
Overall Data:
As for the linear regression for the entire dataset - 
Close to 0: 0.03 (Overall Data for the entire dataset)
Explanation: The R-squared value of 0.03 indicates that only about 3% of the variability in stress levels can be explained by daily steps for the overall dataset, suggesting a weak relationship.
Therefore, for all linear regression outcomes, we shouldn’t rely on data solely on daily steps to predict or explain stress levels; other factors are likely influencing stress levels.


### Affect of Age
Age vs. Sleep Quality:
• For male sleep quality, the R-squared value is 0.0771, suggesting that approximately 7.71% of the variability in male sleep quality can be explained by age.
• The R-squared value for female sleep quality is 0.2066, indicating that around 20.66% of the variance in female sleep quality is accounted for by age.
• When considering both genders, the overall R-squared is 0.2244, meaning that the model explains approximately 22.44% of the variance in sleep quality based on age.

These findings indicate that age has some association with sleep quality, yet a significant portion of the variability remains unexplained. The R-squared values are relatively low, indicating that age alone may not be a strong predictor of sleep quality, and it’s helpful to explore other variables influencing sleep quality.


T-test results:
T-statistic: -5.859317976055214
P-value: 1.078122839334259e-08 
The negative T-statistic means that, on average, females have better sleep quality than males. The small P-value strongly supports this, indicating a significant difference in sleep quality between males and females. Therefore, it seems like females generally sleep better than males.

### Affect of Blood Pressure

Using Group By - data was aggregated first by gender, and then by blood pressure categories. The dataset includes participants with normal, elevated, and hypertension blood pressure measurements. In the data provided, we notice that the majority of study participants experience hypertensive blood pressure - which may influence the findings mentioned below.

First, we observe that there are no Female participants in the study with elevated Blood Pressure. When comparing Sleep Quality and Stress Levels (both qualitative assesments 1-10), we observe little difference for Blood Pressure groups. Surprisingly, we find there is little difference in the average Physical Activity levels reported by each group. Specifically for the male participants, the groups experience elevated and hypertension Blood Pressure levels average more daily physical activity than those in the normal range. Our team speculated whether this related to male's general tendency to be more reactive in their health care - increasing Activity Levels after experiencing Blood Pressure increases. 

Finally, in this sample data set, Female participants on average get better Quality Sleep and have lower Stress Levels - again, with little observable impact from blood pressure. We do not find Blood Pressure to be a good predictor for the other data tracked in this dataset.

### Affect of Gender
The p-values for various t tests were calcultaed in an attempt to identify if there is a significant difference between male and female data.  With p-values less than .05 we can see no statistical difference between them for sleep duration and quality of sleep. There are statistical differences in physical activity and daily steps. This shows that it is dependent on category if male vs female plays a role in the results. The P-values are as follows:
 Male vs Female Physical Activity: P-value=0.9776
Male vs Female Sleep Duration: P-value=0.0189
Male vs Female Quality of Sleep: P-value=1.0781e-08
Male vs Female Daily Steps: P-value=0.7801

### Affect of BMI
BMI by physical activity and gender gave answers that showed that the gender of the person was significant. First the data was cleaned again as our information used multiple names for the same information. Both "Normal & "Normal Weight" as well as "Obese" & "Overweight". The result of the consolidation of the data clearly showed results: "Normal" showed a significantly higher acivity level for males, whereas "Overweight" females showed a significantly higher activity level.

## Conclusion
In conclusion, we came to the following conclusions regarding our initial questions.
(1) How does sleep relate individually to level of fitness during the day?
There was a slight positive correlation between amount of sleep and physical activity during the day.
(2) How does sleep relate to general stress levels?
Overarchingly, study participants who experienced 8 or more hours of sleep had the lowest (3 and 4) recorded stress levels. There is a strong line of regression showing the relationship between decent sleep and lower stress levels. We do note, however, that the majority of the study participants had elevated or hypertensive blood pressure, and that may affect their physical activity and their reported stress level.
(3) Does gender and age affect the variables in a statistically significant way?
We found that as age increased, so did a positive relationship with sleep and phsyical activty. While we do not have data on it, this may be caused by generally being more financially stable as one ages and solidifies their career, as well as having less stress as one moves out of the child-rearing age.
Additionally, male participants showed that more phsyical activity led to lower stress levels, whereas female participants displayed the opposite relationship, where phsyical activity increasing also increased their stress levels. Both of those relationships may have influenced the individual's sleep.
We also acknowledge that the statistical randomness of our data set may be called into question, as the occupations of all the study participants fall into many of the same fields, as well as the amount of study participants with normal blood pressure is shockingly low. Many of the participants of the study, 41.5%, had a diagnosed sleep disorder which also could affect the specific sleep relationships we were investigating.
