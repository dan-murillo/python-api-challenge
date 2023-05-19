# Analysing the weather variables that latitude can predict and finding my ideal holiday cities (*Challenge 6*)

This repository contains a mini-project in which a 603 cities dataset was generated. The data was analysed the influence of the equator and how well latitude could predict four different weather variables.

## Author

Daniel Ramón Murillo Antuna: [@daniel-r-murillo-antuna](https://www.github.com/daniel-r-murillo-antuna)

## Repository and project description

Most people in the world have learnt important facts about the Earth at some point in their life. For example, it is common knowledge that the equator is the imaginary line that divides the Earth into two hemispheres: northern and southern. The equator is at an equal distance from the North and South Poles. Also, it is known that, as one approaches the equator, the weather gets hotter. However, it is not common to test those kinds of facts oneself, and verify from where that knowledge comes.

### Study's purpose:

This mini-project sought to find the data that made that common knowledge possible and went beyond by analysing the maximum temperature, humidity, cloudiness, and wind speed in terms of the equator and whether latitude is a good predictor of those weather variables. The variables were all recorded at a specific moment in time. A second aim was to take this opportunity and find and map my ideal destinations in the world, based on arbitrary limitations to the four previously mentioned variables.

### Summary of the study's conclusions:

Four conclusions were drawn in terms of the first objective:

1. ***The most important conclusion of the analysis is corroborating the existence of the equator and the two hemispheres by looking at latitude and the recorded maximum temperature. Not only does latitude explain about two thirds of the variation in the maximum temperature, but also there is a strong relationship between both variables, which changes between positive and negative on the equator***: latitude and the recorded maximum temperature are tightly related worldwide. However, this relationship changes directions on the equator. North of that line, the relationship between both variables is negative, which means that, as latitude rises, the maximum temperature drops. The opposite direction is also true: as latitude decreases, the maximum temperature increases. This is because there is a strong statistically significant negative correlation between both variables —*r*(539) = -.84, *p* < .001. Additionally, in that hemisphere, latitude is a very good and significant predictor of the maximum temperature because the former predicts about 70.8% of the variation in the latter. In the southern hemisphere, nevertheless, both variables have a different relationship. Both latitude and the maximum temperature either rise or fall together. This is because they are strongly, significantly, and positively correlated in that part of the world too —*r*(539) = .78, *p* < .001. Latitude in this hemisphere predicts about 60.7% of the variation in the maximum temperature.


2. ***Latitude can very weakly predict humidity, and the equator does not seem to play an important role in that relationship***: latitude is a very weak predictor of humidity worldwide because, although both variables are significantly related, their relationship is not strong. As one of the variables considerably grows, the other one just slightly increases. Conversely, as one of them substantially decreases, the other one just slightly drops. This is because, in both hemispheres, a very weak statistically significant positive correlation latitude and humidity was found. Furthermore, in the northern hemisphere, the former seems to predict only about 3.8% of the variation in the latter, and in the southern hemisphere, that percentage drops to 3.5%. Therefore, there are more important variables than latitude that are related to humidity.



3. ***Similarly, latitude can also very weakly predict cloudiness, and the equator has no apparent effect on that relationship***:

Latitude and cloudiness are also very weakly related.
In both hemispheres, there is a very weak statistically significant positive correlation between the variables. In the northern hemisphere, latitude predicts about 2.3% of the variation in humidity, and that percentage grows to about 5.4% in the southern hemisphere. Latitude is a very weak predictor of cloudiness.



lat vs wind speed
Finally, latitude and wind speed have a weak relationship.
In the northern hemisphere, there is a very weak statistically positive correlation between the variables. This means that both variables increase together. Latitude predicts only about 1.9% of the variation in wind speed.
Moreover, in the southern hemisphere, there is a somewhat stronger, but still weak statistically negative correlation between the variables. This means that as latitude increases, wind speed decreases and the opposite direction is also true. Latitide better predicts the variation in wind speed in this hemisphere, as the percentage is somewhat larger: 9.3%.
Latitude is a weak predictor of wind speed.








Set a randomly generated seed to get consistent results every time this entire code is run. This made my city data pseudo-random, which is not too bad, but -> why? didn't want locations to change every time for this mini-project to ensure every time the whole code is run, the results are consistent; otherwise, with a truly random city dataset, the conclusions drawn from the analysis might not have been correct or reflect the newly generated data (limitation: always analysing and drawing conclusions from the same cities, which is a bias; future studies can get rid of the seed and possibly draw different conclusions)
[While building your script, pay attention to the cities you are using in your query pool. Are you covering the full range of latitudes and longitudes? Or are you choosing 500 cities from one region of the world? Even if you were a geography genius, simply listing 500 cities based on your personal selection would create a biased dataset. Try to think of ways that you can counter these selection issues.]





What is citipy used for? Why would you use it in conjunction with the OpenWeatherMap API? How would you do so?




**Future**: carry out a longitudinal study of the weather variables and see whether the results of regressions change depending on the time of day, the month, the season or maybe even a different confounding variable.




Data's true power is its ability to definitively answer questions. So, let's take what you've learned about Python requests, APIs, and JSON traversals to answer a fundamental question: "What is the weather like as we approach the equator?"

Now, we know what you may be thinking: “That’s obvious. It gets hotter.” But, if pressed for more information, how would you prove that?






1. Capomulin was one of the most effective drugs against SCC, particularly when compared to Ketapril. However, although Capomulin showed very promising results, Ramicane seemed to be more effective at treating SCC.
2. Neither the number of mice tested nor the sex of the mice had an effect on how well each drug performed.
3. About the four most promising drugs, Capomulin, Ramicane, Infubinol, and Ceftamin —*as defined by the company*—, the final tumour volumes of all the mice tested with Capomulin and Ramicane were consistently smaller than those of Infubional and Ceftamin.
4. Although Capomulin works, its tumour-shrinking effects might take time to show.
5. There is a significant relationship between mouse weight and tumour volume; both rise together.

### Study conclusions explained with the results of the analysis:

1. ***Capomulin was one of the most effective drugs against SCC, particularly when compared to Ketapril. However, although Capomulin showed very promising results, Ramicane seemed to be more effective at treating SCC***: Based on the summary statistics, the results were very consistent. Ketapril was the drug with the poorest results, as its mean (55.24 mm<sup>3</sup>) and median (53.70 mm<sup>3</sup>) tumour volume throughout the study were the greatest. This means that the tumours treated with this drug were generally the largest. It also had the highest variability of all the drugs, since its was the most spread; the tumour volume values were overall farther from the mean than the other drugs —*the variance was 68.55 mm<sup>3</sup>, and the standard deviation was 8.28 mm<sup>3</sup>*. On the other hand, Capomulin seemed to have a much lower mean (40.68 mm<sup>3</sup>) and median (41.56 mm<sup>3</sup>) tumour volume. This means that the tumours treated with this drug were mainly much smaller. It also showed a much lower variability because the data was less spread; the tumour volume values were substantially clustered closer to the mean than all but one of the drugs —*the variance was 24.95 mm<sup>3</sup>, and the standard deviation was 4.99 mm<sup>3</sup>*. The drug that surpassed Capomulin's results was Ramicane. The latter seemed to have the most consistent results, as it had the lowest mean (40.22 mm<sup>3</sup>) and median (40.67 mm<sup>3</sup>) tumour volume. This means that the tumours treated with this drug were generally the smallest. Ramicane also had the lowest variability, since the data was the least spread; the tumour volume values were broadly clustered closest to the mean —*the variance was 23.49 mm<sup>3</sup>, and the standard deviation was 4.85 mm<sup>3</sup>*. If the company were to repeat the study, Ketapril's tumour volume would vary the most, as it showed the greatest standard error of the mean (0.60 mm<sup>3</sup>) —*the standard error also suggests that Ketapril's true mean tumour volume value size lies between 54.64 mm<sup>3</sup> and 55.84 mm<sup>3</sup>*. Capomulin would vary much less because it had a much lower standard error of the mean (0.33 mm<sup>3</sup>) —*the standard error shows that Capomulin's true mean tumour volume value size would be between 40.35 mm<sup>3</sup> and 41.01 mm<sup>3</sup>*. Nevertheless, Ramicane would vary the least because it had the lowest standard error of the mean (0.32 mm<sup>3</sup>) —*the standard error indicates that Ramicane's true mean tumour volume value size would lie between 39.9 mm<sup>3</sup> and 40.54 mm<sup>3</sup>*.

2. ***Neither the number of mice tested nor the sex of the mice had an effect on how well each drug performed***: This is because a bar chart, which was plotted to compare the number of mice to the administered drugs by counting how many time points were tested for each regimen, revealed, as expected, that Capomulin had the highest number of mice tested. Ramicane was a very close second —*each drug, Capomulin and Ramicane, were tested on over 200 mice*—, and Ketrapril came third with just below 200 mice. Contrarily, Propriva had the lowest number of tested mice —*just below 150*. A pie chart was plotted to compare the overall distribution of female and male mice in the study. The distribution was even: 51% males and 49% females.

3. ***About the four most promising drugs, Capomulin, Ramicane, Infubinol, and Ceftamin —as defined by the company—, the final tumour volumes of all the mice tested with Capomulin and Ramicane were consistently smaller than those of Infubional and Ceftamin***: This conclusion was reached by creating a graph with four boxplots, one per regimen. The graph showed the distribution of the final tumour volume for all mice in each treatment group, and confirmed an even distribution across drugs, although there was one outlier in the Infubinol distribution. The quartiles and the interquartile range were calculated in order to create that graph.

4. ***Although Capomulin works, its tumour-shrinking effects might take time to show***: That was concluded after looking at a line plot of a random mouse that was treated with Capomulin. The line plot compared the tumour volume and all the time points in the study. The mouse selected had the ID number *l509*. Initially, the tumour volume increased until time point 20. However, after that time point, the volume steadily decreased.

5. ***There is a significant relationship between mouse weight and tumour volume; both rise together***: That was found after generating a scatter plot that compared tumour volume and mouse weight for the Capomulin treatment. The plot showed that as the weight rose, so did the tumour volume. Nonetheless, a correlation needed to be ran to statistically prove whether this trend was significant. The correlation was run. The tumour volume and mouse weight were found to be strongly correlated (*r*(23) = .84, p < .01), which means that their relationship was statistically significant.

### More technical information about how the data was treated before the analysis:

*Part 1*: I received 2 original datasets, one of them contained each mouse's metadata and the other one had the study results. I merged both datasets to create a new Pandas DataFrame, screened the data, and found one duplicated mouse, whose ID number was *g989*. The duplicated information was removed. Altogether, there were 248 mice in the clean DataFrame.

### How the analysis was conducted:

- *Part 2*: I calculated the summary statistics: mean, median, variance, standard deviation, and standard error of the mean.

- *Part 3*: I looked at the number of mice tested among the administered drugs and the sex of the mice overall.

- *Part 4*: I calculated the quartiles and interquartile range, and determined outliers in order to graph four boxplots and look at the distribution of the 4 most promising drugs.

- *Part 5*: I generated a line plot to look at the final tumour volume of a random mouse over all the time points in the study. I also created a scatter plot to find a relationship between mouse weight and tumour volume.

- *Part 6*: I ran a Pearson's correlation to prove whether mouse weight and tumour volume were related.

### Improvements for future analyses:

For future analyses, I would suggest to look at the sex proportions of the mice for each drug regimen to confirm whether different regimens had different proportions. I would also generate more line graphs for a larger sample of random mice to more certainly conclude that the Capomulin's positive effects take time to show. Finally, I would look at maybe a correlation matrix of all the variables tested to confirm whether there are more relationships that need to be analysed.

Contents of the repository:

### The *Pymaceuticals* folder:

It contains a folder that has the two original datasets and a Jupyter Notebook with the data cleanup and the analysis.

## Data Reference

The ficitonal data was generated by [Mockaroo](https://mockaroo.com/), LLC (2022). Realistic Data Generator.

```#Thank you for reading me!```

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)





















