# Google-Data-Analytics-Project-FitBit-Data-

For seeing this project without any compiling, make sure to go to: https://rpubs.com/Jandrez/1024930! 

This is a project from the Google Data Analytics Certification. This project helped me clean code, find a dataset via Kaggle, ask meaningful questions with the given variables, and many others!  


## Objective

This was a project that needed to be done in order to get the Google Data Analytics certification. Here is what I've done:
1. Getting the data via Kaggle, and loading it in PostIt (Originally known as R Desktop).
2. Deciding to select the daily dataset in order to conduct statistical analysis and create various graphs to find trends.
4. I then used statistical techniques such as ANOVA, Regression, and others to answer various questions about the user's sleeping/working out habits.


## Dataset
More info about the dataset can be found here:
- Website: https://www.kaggle.com/datasets/arashnic/fitbit

## Discovery

Here is a small conclusion that I've found based on my findings:
- Pokemon with one type from generation 5-7 has experienced a big nose dive in representation. We can also see Pokemon with two types did also suffer from not having a lot of representation as well.
- Overall, the population between one-type and two-type Pokemon does seem similar until the mentioned nose dive from generation 5-6, where two-type Pokemon have more representation in Pokemon games.
- When conducting a T-test, I found that Pokemon with two-type and one-type are statistically significant from one another. This means that Pokemon with two types, on average, had usually higher stats than pokemon with one type.
- Water types have a big representation at a whopping 10.63%, followed by Normal-types 9.40%. But when it comes to legendary Pokemon, Psychic, and Dragon-types become the most potent (16.84% and 11.05% respectively).
- Shockingly Fire types are not even the top 5 most frequent types despite being the main 3 types to be selected at the beginning of the game as a starter Pokemon. As well as not being a potent type when it comes to legendary Pokemon.
- Every 'Total' stat, on average (per generation/region), for non-legendary-pokemon has been very consistent.
- Same goes for legendary but generation 7th (Alola) has experienced an average total stat of 561 (a huge 10% decrease of the total average of all legendaries)
- Thanks to ANOVA, we now know that a lot of types do contain stats that are statistically significant from one another.
- The Attack stat/attribute for all Pokemon was statistically significant, based on regions/generations. (I assume it is because of the outliers of the different regions/generations)
- We can also see that HP and Defense were the ones that were most statistically significant across different regions(based individually per type).
- Ghost-types have a random distribution of stats than other typings. This means that there may be no way of predicting where what stat/attribute will be more prominent in the next set of generations.


## Dataset

This dataset contains X rows and Y columns for the variables listed below. The following contains stats in Pokemon: A Pokemon has a unique set of stats that contribute to the Pokemon's identity. 

Variable  |Description |
-----|-----|
Total|The accumulation of all the stats below|
HP|Also known as "Hit Points": The Health of the Pokemon |
Attack|The physical attack strength of the Pokemon |
Special Attack|The non-physical attack moves from the Pokemon |
Defense|How much can a Pokemon withstand physical attacks
SpecialDefense|How much can a Pokemon withstand non-physical attacks
Speed|This dictates which Pokemon can attack first
Generation|Where the Pokemon is from. Generation and Region will be used interchangeably.
Type 1 and Type 2 |This is the attribute of the Pokemon. There are 18 types in the world of Pokemon. A Pokemon can have just one typing or two. 
Legendary|This is a True/False statement that says if a Pokemon is a legendary Pokemon or not. 
