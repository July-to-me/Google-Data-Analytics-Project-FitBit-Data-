# Google-Data-Analytics-Project-FitBit-Data-

For seeing this project without any compiling, make sure to go to: https://rpubs.com/Jandrez/1024930! 

This is a project from the Google Data Analytics Certification. This project helped me clean code, find a dataset via Kaggle, ask meaningful questions with the given variables, and many others!  


## Objective

This was a project that needed to be done to get the Google Data Analytics certification. Here is what I've done:
1. Getting the data via Kaggle, and loading it in PostIt (Originally known as R Desktop).
2. Deciding to select the daily dataset to conduct statistical analysis and create various graphs to find trends.
4. I then used statistical techniques such as ANOVA, Regression, and others to answer various questions about the user's sleeping/working out habits.


## Dataset
More info about the dataset can be found here:
- Website: https://www.kaggle.com/datasets/arashnic/fitbit

## Discovery

Here is a small conclusion that I've found based on my findings:
- On average, plenty of participants are getting enough sleep to start their day. We can see that 15/24 participants do reach the “ideal” 7-8 hours of sleep, but we can see one of them (participant X-5328) goes above and beyond in their rest! I would love to have more data to see why the other 8 participants do not me the average amount of sleep on average.
- As shown in the line graphs, we can see that Sunday is normally the day when all of our participants are catching up on their sleep. I assume that many of them do have the normal 9-5 full-time jobs, and are getting ready for Monday. The one day that I found interesting is how Wednesday is ranked number 2 when it comes to the most amount of sleep out of the 7-day week.
- As shown in the line graphs, we can see that Saturday has the most amount of steps on average. This means that many of these participants are very active on Saturdays! I am amazed how Sunday, on average, contains the least amount of steps. I assume it is because of how many will try to prepare for the upcoming week.
- Totaltimeasleep and total steps are negatively correlated with one another (-0.1721427), I was expecting this to be more negatively correlated with one another, but it would make enough sense that both variables are not highly correlated with one another given there are other more potent variables.
- When we were able to do an ANOVA test for two variables. We can see that it is very dependent on how many calories the participant burned, as well as the amount of sleep they had. This means that at least one of the predictor variables is significantly different from other levels (for both variables, in their own ANOVA tests). We would be able to follow up with a posthoc test in order to see which predictors are significantly different from one another.
- When plotting the calories vs the intensity of activity level, we can see that, on average, the moderately intense walk is actually damaging the prediction of our linear regression. This is most interesting since it would be safe to assume that the more intense a workout is, the more calories one will burn. But this is not the case as shown in the calories vs totalsteps graph that has activity_level highlighted. Another thing to note is how huge the “cone” is for the very intense level, I assume it is because many bodies will respond to the very intense activities/workout differently (and not in a good way).
- Another thing to note is a lot of data was probably taken out. Data such as the participant’s age, sex, lifestyle, R.E.M, Deep, Light sleep, and diet were missing during this test. I can understand that writing down one’s diet is very time-consuming, but the other variables may not be too time-consuming. I would’ve appreciated it if there was a little bit more information about each participant’s lifestyle since it would’ve helped me provide a better story in this statistical analysis. That, and how some of the data is not there or it was just logged in. This is something that I would’ve enjoyed looking in, but I cannot conduct any findings if the majority did not log it in.



## Dataset

This dataset contains 940 rows and 15 columns for the variables listed below (I've used the daily_activity data frame). The following contains a brief description of what are the variables:

Variable  |Description |
-----|-----|
ID|The identification of the user|
Activity_date|The date when the data was collected|
Total_steps|The number of steps the user has taken for that day|
Total_distance|The distance covered for that day |
Tracker_distance|The distance the tracker was able to track 
Very_active_distance|The intensity of the distance walking and how much the user walked said intensity
Moderately_active_distance|The intensity of the distance walking and how much the user walked said intensity
Light_active_distance	|The intensity of the distance walking and how much the user walked said intensity
Sedentary_active_distance|The intensity of the distance walking and how much the user walked said intensity
Very_active_minutes|The total amount of time the user was able to walk that specific intensity 
Fairly_active_minutes|The total amount of time the user was able to walk that specific intensity 
Lightly_active_minutes|The total amount of time the user was able to walk that specific intensity 
Sedentary_minutes|The total amount of time the user was able to walk that specific intensity 
Calories|The total amount of calories burned off when exercising 
