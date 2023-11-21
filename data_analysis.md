# Group 6 - Project 1

## Data Cleaning
	To understand our data, some quick visualizations were run. Sophie Geister-Jones created visuals of the dataset based on gender, age, blood pressure, and sleep disorder diagnosis. We noticed that there seemed to be a larger amount of study participants that have hypertensive blood pressure than would be expected.
	Bob Erickson did the majority of cleaning the data when we were all first exploring it. He split the blood pressure into two columns that were labeled as Systolic and Diastolic. That allowed Sophie Geister-Jones to create a qualitative column for blood pressure that labeled the data as “low,” “normal,” “elevated,” or “hypertensive.” Additionally, Erickson also cleaned up the Sleep Disorder column by replacing “NaN” values with “No Diagnosis”.

## Analysis Questions
	The Sleep Health and Lifestyle Dataset uploaded on Kaggle.com by Laksika Tharmalingam (2023) contained data on 374 individuals’ gender, age, sleep duration and quality, stress level, physical activity level, blood pressure, and BMI standing. After examining the raw data, we had three questions we wished to investigate: (1) How does sleep relate individually to level of fitness during the day? (2) How does sleep relate to general stress levels? (3) Does gender and age affect the variables in a statistically significant way?
  We hypothesized that the best way to search for any potential relationships was to analyze the relationship between sleep and fitness, sleep and stress, and stress and fitness and to see if any one relationship had a stronger correlation than others.

### Sleep and Physical Activity
We examines the relationship between sleep and fitness level. Sleep duration is measured in hours and physical activity level is the minutes per day a person engages in physical activity. There are a few potential outliers within the data set that could be skewing results as shown in a box and whiskers plot created between the sleep duration and phydical activity level. A scatter plot shows a slightly positive correlation. These graphs show that for the extreme physical activity levels there are wide ranges of sleep duration. In general we noted higher physical activity level correlates with sleep duration.
### Sleep and Stress Levels
There's a negative correlation between sleep duration and stress level:
• Having longer sleep durations might be associated with lower stress levels, indicating the potential importance of sufficient sleep in managing stress.
• Similarly, shorter sleep durations might be associated with higher stress levels, suggesting that inadequate sleep could contribute to increased stress levels.

Stress Level Frequencies :
• Male are facing more stress levels compared to female's.
• Female stress levels are very low based on the available data.

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

### Affect of Gender
The p-values for various t tests were calcultaed in an attempt to identify if there is a significant difference between male and female data.  With p-values less than .05 we can see no statistical difference between them for sleep duration and quality of sleep. There are statistical differences in physical activity and daily steps. This shows that it is dependent on category if male vs female plays a role in the results. The P-values are as follows:
 Male vs Female Physical Activity: P-value=0.9776
Male vs Female Sleep Duration: P-value=0.0189
Male vs Female Quality of Sleep: P-value=1.0781e-08
Male vs Female Daily Steps: P-value=0.7801

### Affect of BMI
BMI by Physical Activity & Gender gave answers that showed that the gender of the person was significant. First the Data was cleaned again as our information used multiple names for the same information. Both "Normal & "Normal Weight" as well as "Obese" & "Overweight". The result of the consolidation of the data clearly showed results. "Normal" showed a significantly higher acivity level for Males, whereas "Overweight" Females showed a significantly higher activity level. 


## Conclusion
