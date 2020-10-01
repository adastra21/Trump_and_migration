# FinTech540: Project 1

## Problem: Predicting Trump Support from Migration Trends
I used a k-nearest neighbors model to predict whether a county will vote for Trump given its recent migration history. I measured migration history by averaging the percentage change in migration over the five years from 2011 to 2015 for both domestic and international migration. I measured support for Trump by looking at whether a county voted for Trump in the 2016 Presidential Elections.

### Datasets
US Census population estimates with migration trends (Source: Dr. Lenz, Duke University)
US Voting data from the 2016 Presidential Elections (Source: https://github.com/tonmcg/US_County_Level_Election_Results_08-16)

### Results
I was able to predict with 85% accuracy whether a county will vote for Trump. However, the AUC was only 0.57. The performance of the model was very sensitive to change in the values for nearest neighbors, and did not converage until n=42.

### Future improvements
* Use lagged variables instead of five year averages
* Add more migrant variables, esp. migration by age group or religion
* Use data from all counties, instead of those with domestic flight
* Use a bigger dataset with data for 2008, 2012 and 2016 Presidential Elections
* Experiment with Random Forests and SVM
