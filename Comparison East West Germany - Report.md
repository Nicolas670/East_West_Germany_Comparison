
# Report: Comparison East vs West German Cities:

#### For my final Assignment I plan on comparing two cities of each, east and west Germany. On the Side of east Germany standing are Dresden and Leipzig. Representing West Germany are Frankfurt and Nürnberg.

### 1. Interest:

This topic could be of interest for anybody who has to choose between living in either of these cities, or potentially for the German Government.
Since the reunion of Germany in 1990 the east seems to have struggled to catch up.
This has a variety of reasons and shall not be discussed any further in this eploration, since it would be far to much to consider.
Just Comparing the Cities on a few basic criteria could get very interesting though.

##### Why would the Germany Government have an interest in such an eploration?
Since the reunion Germans pay a Tax called "the soli" which is used to pay for repairing the decay that occured in east germany during the time germany was divided.
There is a debate in Germany, wether this tax should be abolished or not.
Exploring wether the cities of east Germany have catched up with the west may be one criteria of abolishing the tax.

#### The four selected cities:
![map_germany](https://user-images.githubusercontent.com/61230508/75711465-bfd66400-5cc6-11ea-97bb-6953332f7fd0.PNG)

### 2. Data:
#### For this exploration we will need:
- Coordinates of the 4 Cities: Dresden, Frankfurt, Leipzig and Nürnberg
- Categories in which we will compare the cities: Culture, Education, Leisure and Food / Restaurants
- Data for each category

We can collect the needed data for each categorie and city from Foursquare.
Since this is only a quantitative analysis and not considering the quality of each found venue, we do not need any premium requests from Foursquare thus we can go with a free account

The sum of the Criteria is ment to be somewhat representativ of the living quality and diversity in each city.
Especially the number of restaurants (with foreign cuisine) is ment to represent the diversity of the city, whereas the other three criteria encode for living quality and state of a city.
Particularly from Culture and Education one might be able to conclude wether a city needs more funding or already has enough.

### 3. Methodology:

The main work to be done lies in collecting the data from foursquare, reshaping it and visualizing it with folium.

First we will have to collect the location data of each city.

Then define the categories in which we will compare the cities.

Third is actually getting the data from Foursquare and transforming it into a Pandas DataFrame. This tourned out
to be the most labour intense part, since I wanted to make both, the data aquisition, as well as the transforming dynamical,
so that adding or changing the cities won't result in any additional work:

Once the data is nicely sorted in a DataFrame, we have to check, wether the data is correct, anything is missing or some outlyers distort the picture.
![checking_outliers](https://user-images.githubusercontent.com/61230508/75711433-b2b97500-5cc6-11ea-9c48-c1a6cbb543e4.PNG)

Check why Frankfurt seems to have so much more venues:
![map_outliers_frankfurt](https://user-images.githubusercontent.com/61230508/75711746-2fe4ea00-5cc7-11ea-81d1-40909445eef0.PNG)

There are venues shown in Wiesbade, a city next to Frankfurt.
The data we received was therefor too broad. Next step was dropping the venues that were not located directly on one of the four cities. 

Finally visualizing the data to show any possible conclusions that might be drawn.
![comparison](https://user-images.githubusercontent.com/61230508/75711802-44c17d80-5cc7-11ea-8d2c-ef15587cf4cf.PNG)

### Observations:

Nürnberg, Dresden and Leipzig don't seem to be too far apart in regards to the four categories.
Frankfurt on the other hand is an outlier. Espacially in Culture and Restaurants.
I am quite surprised that Frankfurt seems to have so much more Restaurants than the other three cities.
The explanation is to be found in the criteria I picked for the restaurants: 
            "Italian", "Spanish", "Sushi", "Chinese", "Korean", "Indian","African"
These are all foreign cuisines. And since Frankfurt is known to be a particularily multi cultural city it doesn't surprise, that many restaurants of foreign cuisine are to be found there.
Wheras Nürnberg Dresden and Leipzig seem to have less of a cultural variety.

### Restrictions:

In this comparison I chose 4 cities with roughly the same size. It is to be noted though, that that Franfurt has roughly 200k more inhabitants.
A more precise way to look at the data would possibly be calculating the criteria in proportion to population count, or square kilometer.
Also the availability of Jobs, the payment and the living cost contribute a hughe part to the living quality in one place. This hasn't been taken into account in this exploration.

### Conclusion:

It seems that Frankfurt has defnetly a lot more variety going than the other three cities.
Between Nürnberg, Dresden and Leipzig doesn't seem to be a big difference though. 
We could conclude from this, that living quality in the cities of east germany matches this of west german cities.
That is for the big cities. I don't think one could draw reliable conclusions from this for the whole east / west german perspective.
To do this one had to take into account the population density in the areas as well.
Nevertheless it was interesting to see in how the cities compare to each other.


```python

```
