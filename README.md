# Safety Inspection in Restaurants across New York City

In this work we look at the restaurant inspection data from New York City between 2009-2014. The entire analysis is done using SQL. The dataset contains 5 tables:

1. `webextract`: main table containing data about the ID, name, location (including zipcode and borough), primary cuisine served, inspection date, violation code, score and grade of the restaurants. In total there are 16 columns and 531,935 rows including information about 24,361 restaurants. 
2. `cuisine`: secondary table containing the code and name of the cuisine served by the restaurant. In total there are 85 different cuisines.
3. `violation`: table containing description of violations committed by restaurants. The total number of violation codes are 174.
4. `boroughs:` table containing id and names of 5 boroughs of NYC.
 
The first goal of the work is to look at the areas in the city by zipcodes and boroughs that have the highest and lowest inspection scores. East Village (East 12th and 3rd Ave.) and Upper West Side (West 54th and 9th Ave.) have the most number of restaurants at 658 and 648 respectively. Borough Park (51st Street and 13th Ave.) and Bensonhurst (East 9th and Ave. K) have the lowest number of restaurants with 101 each. The western and southern parts of the city scored higher on inspection scores whereas the lower scores were located in the eastern parts of the city. Flushing and Astoria in Queens with 187 and 110 restaurants respectively have the highest inspection scores indicating the safest areas to eat. Bronx city and Chelsea (West 30th and 6th Avenue) have the lowest scores. Amongst the 5 boroughs, Staten Island is the safest and the Bronx is the least safe place to eat. 

We then look at the cuisines that have the highest and lowest number of violations. In total, American cuisine had the most number of restaurants (6154), followed by Chinese (2395) and Pizza (1191). The cuisines with the least violations are: hotdogs, sandwiches, donuts and ice cream/gelato/frozen yogurt. The most violations occured for Creole, Chinese/Japanese, Portuguese and Pakistani with 5 times more violations per year than the safest cuisines. 

Finally, we look at the most disproportionate violations in cuisines, i.e. the violations that occur higher than usual in certain cuisines. In general, 'Non-food contact (such as door knobs, chairs, pickup counters, shared spaces, telephones, cash registers, etc.) surface improperly constructed' was the most violated code followed by places not being vermin proof. The topmost disproportionate violations were: 
* Workers not using proper utensils to avoid bare hand contact with food for Japanese food,
* Missing signs for choking first aid, alcohol and pregnancy warning, inspection report sign for Café/Coffee/Tea places,
* Food protection certificate not held by the restaurant for places serving Juice, Smoothies, Fruit Salads. 
