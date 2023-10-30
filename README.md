# project-1


# Q1 Are movies that are more popular rated higher than movies that are less popular?
We categorised the movies into two groups based on the median, which are labelled as "more popular" and "less popular." The aim of these categorizations is to reflect the hypothesis that higher-rated movies might be considered more popular because of increased viewer interest. We consider that the data doesn't follow a normal distribution and that movies with more ratings are generally more popular. To compare the movie rating between these categories, we chose to employ a two-sample T test, chosen for its suitability in comparing non-parametric data, even in cases where the data does not follow a normal distribution.

After performing the T test, which evaluates the difference in median between these groups, the team obtained a p-value of 6.15e-35 and t-statics of 13.40. This p-value suggests that movies with higher popularity ratings tend to have higher viewer ratings compared to movies with lower popularity ratings.

So, based on the p-value that we got, it strongly indicates a substantial difference in viewer ratings between movies labelled as "more popular" and "less popular." It is consistent with the hypothesis.


# Q2 Are movies that are newer rated differently than movies that are older?
Based on the release years of movies, we decide to divide the dataset into two groups, which are labelled as “newer movies” and “older movies”. We still use a two sample T test here. We base on the median release year to divide these two groups. The median was computed after careful consideration of potential duplicate years (for example, there were 29 movies released in 1999) and their impact on the split. The two-sample t-test aimed to determine if there was a significant difference in the mean ratings between “newer movies” and “older movies” by assuming the data approximated a normal distribution.


The result was an average rating of 2.76 for the “newer movies” and 2.67 for “older movies.” The t test produced a t-statistic of 3.65 and a p- value of 0.00028. Compared against a significant level of 0.005, it leads to the rejection of the null hypothesis. This proves the mean ratings between “newer movies” and “older movies” are significantly different.


The result strongly shows a significant distinction in viewer ratings between “newer movies” and “older movies”.


# Q3 Is enjoyment of ‘Shrek (2001)’ gendered?
We conducted a two-sample t-test to analyse the ratings of ‘shrek(2001)’ by male and female viewers. We tried to find the ratings of male and the ratings of female viewers and to evaluate differences between these two groups. To ensure the integrity of analysis, we remove rows with missing values.

The result: The t test produced a t-statistic of 1.17 and a p- value of 0.25. Compared with a significant level of 0.005, there is no strong evidence to reject the null hypothesis, so there is no significant difference in the ratings of  ‘shrek(2001)’ between male and female viewers


# Q4 What proportion of movies are rated differently by male and female viewers?
We assumed that the significance level was 0.005. We conducted the Mann-Whitney U test for each movie and examined potential differences in movie ratings between male and female viewers. This method allows us to compare the ratings of movies based on male and female viewers. The results indicate that the proportion of movies that are rated differently by male and female viewers is 0.125.


# Q5 Do people who are only children enjoy ‘The Lion King (1994)’ more than people with siblings?
We assume that the ratings are independent. We tried to extract the ratings of ‘The Lion King(1994)’, and the status of  ‘only child’. By conducting a two-sample t-test, we decided to divide the dataset into two groups, which are ‘only child’ and ‘with siblings.’ Then compare the ratings between ‘only child’ and ‘with siblings.’ 
The t test produced a t-statistic of -1.88 and a p- value of 0.061. Compared against the significance level, there isn’t significant evidence to support a difference in the enjoyment of ‘The Lion King(1994)’ between  ‘only child’ and ‘with siblings.’ 


# Q6 What proportion of movies exhibit an “only child effect”?
We assumed that the significance level was 0.005. We conducted a Mann-Whitney U test for each movie to compare ratings between viewers who are only children and those who have siblings. and we compared the ratings of movies based on viewers' family background.The results indicate that proportion of movies showing an 'only child effect' is 0.0175


# Q7 Do people who like to watch movies socially enjoy ‘The Wolf of Wall Street (2013)’ more than those who prefer to watch them alone?
We assumed that the ratings are independent and we handled missing values. We selected the relevant columns and split the data into two groups based on viewing preference. We used t-test, since it directly compares the average ratings of 'The Wolf of Wall Street (2013)' between viewers who prefer social watching and those who prefer watching alone. 
We conducted a two-sample t-test to compare the average ratings and calculated the t-statistic is 1.5513309472217705  and p-value is 0.1213910395002074.
The results indicate that the average rating for 'The Wolf of Wall Street (2013)' for those who prefer to watch movies alone is 3.143765903307888 and the average rating for 'The Wolf of Wall Street (2013)' for those who prefer to watch movies in a group is 3.033333333333333. So, the people who liked watching The Wolf of Wall Street (2013) alone had higher average ratings than people who liked watching The Wolf of Wall Street (2013) as a group.


# Q8 What proportion of movies exhibit such a “social watching” effect?
We assumed that the significance level was 0.005. We conducted the Mann-Whitney U test for each movie and identified movies with a significant "social watching" effect based on the significance threshold. This method allows us to compare the ratings of movies based on audience preferences. The results indicate that the proportion of movies showing a 'social watching effect' is 0.025


# Q9 Is the ratings distribution of ‘Home Alone (1990)’ different than that of ‘Finding Nemo (2003)’?
We assumed that the ratings for both movies are independent, and we performed a two-sample t-test to compare their means. We set the significance level (α) to 0.005.This approach allowed for an assessment of whether there is a significant difference in the ratings.
We conducted a two-sample t-test to compare their ratings distributions. The test yielded a t-statistic and a p-value. The t-statistic quantifies the difference in means between the two movie ratings,  p-value represents the likelihood of difference.
After performing the two-sample t-test, we get the T-statistic is 0.6832827583944752 and P-value is 0.495518534379527. The results indicate that there is a significant difference in the ratings distribution between 'Home Alone (1990)' and 'Finding Nemo (2003)'.


# Q10 There are ratings on movies from several franchises ([‘Star Wars’, ‘Harry Potter’, ‘The Matrix’, ‘Indiana Jones’, ‘Jurassic Park’, ‘Pirates of the Caribbean’, ‘Toy Story’, ‘Batman’]) in this dataset. How many of these are of inconsistent quality, as experienced by viewers? 
We assumed that the average ratings of movies within each franchise would be relevant for evaluating quality consistency. We performed one-sample t-tests for each franchise and we set a significance level of α = 0.005. This approach allowed for a direct comparison of franchise ratings against the overall dataset, enabling us to identify franchises with potentially inconsistent quality
The average ratings for each of the specified franchises were as follows:
Star Wars: 2.78
Harry Potter: 2.73
The Matrix: 2.76
Indiana Jones: 2.72
Jurassic Park: 2.77
Pirates of the Caribbean: 2.77
Toy Story: 2.79
Batman: 2.74
We conducted t-tests for each franchise to compare their average ratings with the overall dataset's average rating (2.75). We conclude that no specific franchises exhibit inconsistent quality in movie ratings. 


