# Safety Inspection in Restaurants across New York City

In this work we look at the restaurant inspection data from New York City. The entire analysis is done using SQL. The dataset contains 5 tables:

1.   `webextract`: main table containing data about the ID, name, location (including zipcode and borough), primary cuisine served, inspection date, violation code, score and grade of the restaurants.
2.   `cuisine`: secondary table containing the code and name of the cuisine served by the restaurant.
3.  `action`: table containing description of action taken against violations.
4. `violation`: table containing description of violations committed by restaurants.
5. `boroughs:` table containing id and names of 5 boroughs of NYC.

The goal of the work is to look at the areas in the city by zipcodes and boroughs that have the highest and lowest inspection scores. We then look at the cuisines that have the highest and lowest number of violations. Finally, we look at the most disproportionate violations in cuisines, i.e. the violations that occur higher than usual in certain cuisines.

* The western and southern parts of the city scored higher on inspection scores whereas the lower scores were located in the eastern parts of the city. 
* Amongst the 5 boroughs, Staten Island has the highest and the Bronx the lowest inspection scores.
* The cuisines with the least violations are: hotdogs, sandwiches, donuts and ice cream/gelato/frozen yogurt. The most violations occured for Creole, Chinese/Japanese, Portuguese and Pakistani.
* The topmost disproportionate violations were:
    * Workers not using proper utensils to avoid bare hand contact with food: Japanese
    * Missing signs for choking first aid, alcohol and pregnancy warning, inspection report sign: Café/Coffee/Tea
    * Food protection certificate not held by the restaurant: Juice, Smoothies, Fruit Salads. 
