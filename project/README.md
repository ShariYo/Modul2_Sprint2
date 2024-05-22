
# Fast Food Market and Cookie Cat game analysis

This study includes mostly A/B test with analyzing experiments, conducting statistical tests and calculating confidence intervals. Also, a dashboard of Fast Food Market is created. The study itself consists of two parts:  
- 1 part - Fast Food Marketing Campaign A/B test;  
- 2 part - Cookie Cats game A/B test.  
Brief information about each of parts:  
**Fast Food Marketing**: A fast-food chain plans to add a new item to its menu. However, they are still undecided between three possible marketing campaigns for promoting the new product. A different promotion is used at each location, and the weekly sales of the new item are recorded for the first four weeks.  
*The goal of this A/B test is to analyse, which promotion (1, 2, 3) would give the most significant positive result in sales.*  
**Cookie Cats game**: This dataset includes A/B test results of Cookie Cats game to examine what happens when the first gate in the game was moved from level 30 to level 40. When a player installed the game, he or she was randomly assigned to eighter gate 30 or gate 40.  
*The goal of this A/B test is to analyse in which level (30 or 40) player should encounter gate to keep players longer in the game.*


## Data source

Given data source can be found at Kaggle with the two links provided below:

  **Fast Food Marketing**  

  https://www.kaggle.com/datasets/chebotinaa/fast-food-marketing-campaign-ab-test/data  

  **Cookie Cats game**  

  https://www.kaggle.com/datasets/mursideyarkin/mobile-games-ab-testing-cookie-cats/data



## Main functions/libraries used for data analysis:  
### Link to dashboard:  
https://lookerstudio.google.com/reporting/ae82193e-2d24-463a-b404-3bfe265b4d41
### Libraries:  
- numpy;
- pandas;
- matplotlib.pyplot;
- seaborn;
- cleaner (internal custom function);
- scipy.stats;  
- statsmodels.stats.proportion

### Plots:
- sns.kdeplot();
- sm.qqplot();
- sns.histplot();
- sns.heatmap();
- sns.barplot();
### Files:
- WA_Marketing-Campaign.csv;
- cookie_cats.csv;

## Summary

In this project two datasets were analysed throught different slices of data using A/B Test.  
- For Fast Food Marketing Campaign A/B test, a two sample independent test for the mean has been chosen to reject or accept null hypothesis. Null hypothesis says *there is no difference in sales between promotion 2 and promotion 3 in medium size markets*. At the end of calculations, Null hypothesis was rejected, which meant that there was a significant difference in sales between 2 and 3 promotion in medium size markets.  
- For Cookie Cats game A/B test, a two sample independent test for proportion as well as Bootstrap have been chosen to reject or accept null hypothesis. Null hypothesis says *there is no significant difference in 7 days retention success rate between gate 30 and gate 40*. Null hypothesis was rejected, which meant that there was a significant difference in 7 days retention success rate between gate 30 and 40.  
- An interactive dashboard was created to show Fast Food Marketing on different weeks through different sizes of markets. To show weekly income, KPI stats included.

