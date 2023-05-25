# Analysing the weather variables that latitude can predict and finding my ideal holiday cities (*Challenge 6*)

This repository contains a mini-project in which a 541 cities dataset was generated. The data were used to analyse the relationship between the equator and the weather as well as to determine whether latitude could predict four different weather variables.

## Author

Daniel Ramón Murillo Antuna: [@daniel-r-murillo-antuna](https://www.github.com/daniel-r-murillo-antuna)

## Repository and project description

Most people in the world have learnt important facts about the Earth at some point in their life. For example, it is common knowledge that the equator is the imaginary line that divides the planet into two hemispheres: northern and southern. That line is at an equal distance from the North and South Poles. Also, it is known that, as one approaches the equator, the weather gets hotter. However, people tend neither to test those kinds of facts themselves nor to verify from where that knowledge comes.

### Study's purpose:

This mini-project sought to find data, which made that common knowledge possible and went beyond by analysing the maximum temperature, humidity, cloudiness, and wind speed in terms of the equator and whether latitude is a good predictor of those weather variables. The variables were all recorded at a specific moment in time. A second aim was to take this opportunity to find and map my ideal destinations in the world, based on arbitrary limitations to the four previously mentioned variables.

### Summary of the study's conclusions:

Four conclusions were drawn in terms of the first objective:
1. The first and most important conclusion of the analysis was corroborating the existence of the equator and the two hemispheres by looking at latitude and the recorded maximum temperature. Not only is latitude a good predictor of the maximum temperature —the former explains about two thirds of the variation in the latter—, but also there is a strong relationship between both variables, which changes on the equator.
2. The relationship between latitude and humidity is not important, and the equator does not seem to play an important role in that relationship.
3. Similarly, latitude can also very weakly predict cloudiness, and the equator has no apparent effect on that relationship.
4. Finally, latitude and wind speed also have a very weak relationship, although the equator does seem to have some effect on that.

### Study conclusions explained with the results of the analysis:

1. ***The first and most important conclusion of the analysis was corroborating the existence of the equator and the two hemispheres by looking at latitude and the recorded maximum temperature. Not only is latitude a good predictor of the maximum temperature —the former explains about two thirds of the variation in the latter—, but also there is a strong relationship between both variables, which changes on the equator***: latitude and the recorded maximum temperature are tightly related worldwide. North of that line, the relationship between both variables is negative, which means that, as latitude increases, the maximum temperature decreases. The opposite direction is also true: as latitude decreases, the maximum temperature increases. That is due to a strong, statistically significant, *negative* correlation between both variables (*r*(539) = -.84, *p* < .001). In the northern hemisphere, latitude predicts about 70.8% of the variation in the maximum temperature. Interestingly, in the southern hemisphere both variables have a different relationship. Both latitude and the maximum temperature either rise or fall together. This is because, although they are also strongly and significantly correlated, as in the northern hemisphere, the correlation is *positive* south of the equator (*r*(539) = .78, *p* < .001). In the southern hemisphere, latitude predicts about 60.7% of the variation in the maximum temperature.

2. ***The relationship between latitude and humidity is not important, and the equator does not seem to play an important role in that relationship***: latitude is a very weak predictor of humidity worldwide, since both variables are only slightly related. On both sides of the equator, as one of the variables considerably grows, the other one very slightly increases. The same relationship can be seen when both variables decrease. This is because, in both hemispheres, a very weak, statistically significant, *positive* correlation between latitude and humidity is found (northern: *r*(539) = .19, *p* < .001; southern: *r*(539) = .19, *p* < .05). Furthermore, while in the northern hemisphere latitude seems to predict only about 3.8% of the variation in humidity, in the southern hemisphere that percentage drops to 3.5%. 

3. ***Similarly, latitude can also very weakly predict cloudiness, and the equator has no apparent effect on that relationship***: latitude and cloudiness are also very weakly related. In both hemispheres, there is a very weak, statistically significant, *positive* correlation between both variables (northern: *r*(539) = .15, *p* < .001; southern: *r*(539) = .23, *p* < .01). In the northern hemisphere, latitude predicts about 2.3% of the variation in humidity, and that percentage grows to about 5.4% in the southern hemisphere.

4. ***Finally, latitude and wind speed also have a very weak relationship, although the equator does seem to have some effect on that***: in the northern hemisphere, there is a very weak, statistically significant, positive correlation between both variables (*r*(539) = .14, *p* < .01), which means that both variables either increase or decrease simultaneously. However, below the equator that relationship changes direction. In the southern hemisphere, there is a somewhat stronger, but still weak, statistically significant, *negative* correlation between latitude and wind speed (*r*(539) = -.30, *p* < .001). Hence, when the former increases, the latter decreases or when the former decreases, the latter increases. Although weak, this relationship also seems to prove the existence of the equator. North of that line, latitude predicts only about 1.9% of the variation in wind speed, whereas in the south, the percentage is somewhat larger: 9.3%.

### How the analysis was conducted:

This mini-project included two parts:

- *Part 1*: A Python script was created to visualise the weather of over 500 randomly selected cities, which varied in distance from the equator. *Numpy* was used to generate 1500 random latitude and longitude combinations —*a randomly generated seed was used to get consistent results every time the entire code is run*. Out of those combinations, only 603 cities were found with the *CitiPy* library. The *OpenWeatherMap API* was used to obtain weather data about the 603 cities found, but information was found about only 541. Scatter plots were generated and linear regressions run to analyse the relationship between latitude and the four other variables —maximum temperature, humidity, cloudiness, and wind speed. All of the data was exported to a CSV file.

- *Part 2*: The CSV created in part 1 was read and all the cities mapped —*the size of the point was proportional to the humidity in each city*. I filtered the cities by my ideal weather conditions: maximum temperature between 26ºC and 30ºC, highest wind speed of 5 m/s, lowest humidity of 40%, and greatest cloudiness of 40%. Only 15 cities met those conditions. I used the *Geoapify API* to find the first hotel located within 10 km of each city's coordinates. I found hotel information of 9 cities, so I created a *Pandas* DataFrame, added to the DataFrame the data I found, and mapped the destinations with *hvPlot*.

### Improvements for future analyses:

While testing the code of this mini-project, I observed that the existence of equator is best proved by looking at latitude and the recorded maximum temperature at given times, although I did not record all of those times. Future studies could carry out a 24-hour study to see whether this observation is true. They could also carry out a longitudinal study of the weather variables and see whether the results of regressions change depending on the month, the season or maybe even discover a different —*possibly confounding*— variable not identified in my analysis. Also, they could get rid of the random seed to make their experiment truly random, instead of pseudo-random, and run the code many times to corroborate the conclusions I found. Although my analysis included cities from many regions of the world, future studies could maybe also include a fuller range of latitudes and longitudes by analysing a greater number of cities.

Contents of the repository:

### The *WeatherPy* folder:

It contains the two Jupyter Notebooks with the Python code of parts 1 and 2 of my analysis.

### The *output-data* folder:

It contains the CSV file I generated and the images of the four scatter plots I graphed.

## Data Reference

All the data were generated during the mini-project, hence, there are no data references other than the libraries and APIs used in the code: CitiPy, the OpenWeatherMap API, and the Geoapify API.

```#Thank you for reading me!```

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)
