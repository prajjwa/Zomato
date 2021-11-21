

This Project Involved doing case study on restaurants on india via zomato API.

Skills Involved:
Python
Numpy
Pandas
APIs

**Prajjwal Singh**

**Plot the bar graph of a number of restaurants present in Delhi NCR vs Rest of India.**

Ans:: First I have filtered out all countries which is not having Country Code as 1. Next, I have

made one set wherein I kept all the cities that are in Delhi-NCR which will help me to segregate

data.

Next I plot bar graph of Delhi ncr and rest of india

**Find the cuisines which are not present in restaurants of Delhi NCR but present in rest of**

**India. Check using Zomato API whether these cuisines are actually not served in restaurants**

**of Delhi-NCR or just it due to incomplete datase**

First i make 2 sets of Delhi ncr and rest of india and then i run a for loop where the data in rest of

india is not in delhi ncr and append this data in a list. And this list contained the cuisines that were in

rest of india not in delhi ncr.

Next i made a request on zomato api and got a json as response and checked if the response had

the data in delhi ncr.

**Find the top 10 cuisines served by a maximum number of restaurants in Delhi NCR and the**

**rest of India.**

After making the two sets of delhi ncr and rest of india i used value counts method on these two set

and got most common cuisines in delhi ncr and rrest of india. And finally plotted the result.





**Write a short detailed analysis of how cuisine served is different from Delhi NCR to Rest of**

**India. Plot the suitable graph to explain your inference.**

From the graph, we can see that North Indian, Chinese Cuisine are servered most in both

places. But number of

restaurants serves has a huge difference, North Indian cuisine is served by more than 3500

restaurants in Delhi NCR

but this data changes drastically in Rest of India, and that is only 350 or so and same goes for

Chinese cuisine.

Third most served cuisine in Delhi NCR is Fast Food wherein Rest India is Continental and

there is some order difference

in terms of restaurant serves. There are total 86 different cuisines that are offered in Delhi-NCR

wherein Rest India offers

70 different cuisines.





**Q2)User Rating of a restaurant plays a crucial role in selecting a restaurant or ordering**

**the food from the restaurant**

**Number of Votes given Restaurant**





To get the idea of rating and how many votes they might have got, I have applied data compression

technique as a number of votes can be so huge for a particular restaurant. To compress the data I

have first added all the votes by the rating and maintain total restaurants which will help me to figure

out the average voting for each restaurant. So first I have made one dictionary which will hold the

rating as key and a total number of votes & restaurant count as a value i.e a list 0th index is total

number of votes and 1st restaurant count. Once I get these detail I can make an average by doing

total\_votes//no\_restaurants so for each restaurant we will get the compressed voting numbers. After

ploting in the graph we can see that those restaurants get more vote they usually got good rating i.e

4- 5 and voting range is 500 - 2000. Now if we see the low rating then we can find that there are less

voting as compare to 4-5 rating range voting. From the above explanation, I can say that if we go

with large number of voting for a restaurant they we will get good food usual.

**Restaurant serving more number of cuisines.**

I have applied the same technique just in this case and for below cases I haven't used any

function to get the desired result. Here I have twicked the scenario little because we need to

check with the number of cuisines so I made number of cuisines as key and I have stored all

the rating given to particular number of cuisines and side by side I have stored the number of

restaurants. After doing this, I am finding the average rating for that particular number of

cuisines right. And rating will lie between the min rating and max rating got by number of

cuisines. To find out the average rating I have used total\_rating/restaurant\_count. After

ploting the detail in the graph we can notice the higher number of cuisines offered more is

the rating. 60 - 80 range has got the higher ratings. But still there are some restaurants after

offering ample number of cuisines still they couldn't get good rating. So it will be better to go

with more number cuisines offered by a restaurant





**Average Cost of Restaurant**

As I have mentioned earlier, I have applied the same logic so I am not re-iterating the same

thing. Here I have used cost of two as the key and store all the ratings for a particular cost

and side by side I have store the count of restaurants inorder to get the average. Once all the

data stored in the dictionary I have found the average by total\_ratings/restaurant\_counts.

After ploting the graph it is indicating that more cost of two more is the rating of the

restaurant. When cost of two gets more than 2000 the rating becomes stagnant i.e we can

say that there is no big fluctuation. So if we select a restaurant wherein cost of two in

between 1000 - 2000 that will provide us good food

**Restaurant serving some specific cuisines**

As earlier, here I have made one dictionary which is storing cuisines and ratings and the

count of restaurants, wherein cuisine works as the key and total\_ratings and number of





restaurant. First I have summed up all the ratings and then I have divided by the total

number of restaurants, which is helping me to get the average rating. Once I got the average

rating for the cuisines I have sorted them in descending order based on their ratings and

after that I have plotted them in bar graph. From bar graph we can see that those restaurants

offering Persian, German, Mordern Indian cusines get the good ratings. So if we good to a

restaurants wherein these cuisines are being offered then there is likely to get good food.

**Find the weighted restaurant rating of each locality and find out the top 10 localities**

**with more weighted restaurant rating?**

As we need to find the weighted ratings for each locality I have used one dictionary which will

store the locality names and it will store all the values of all restaurants present in that

locality. As formulation has been mentioned, I have applied that formula to get the weighted

rating. Once that has been done, I have plotted the graph and from that graph we can see

these are the top 10 localites:

1 Hotel Clarks Amer, Malviya Nagar

2 Aminabad

3 Friends Colony

4 Powai

5 Kirlampudi Layout

6 Express Avenue Mall, Royapettah

7 Deccan Gymkhana

8 Banjara Hills

9 Sector 5, Salt Lake

10 Riverside Mall, Gomti Nagar





**Q3)Plot the bar graph top 15 restaurants have a maximum number of outlets.**

We can get maximum restaurants by applying value counts which groups on the bases of the value

and arranges on the descending basis.

Finally we plot our result.





**Plot the histogram of aggregate rating of restaurant( drop the unrated restaurant).**

As mentioned in the question I need to drop all the unrated restaurants so I have checked the Rating

text column if the text is not Not Rated then consider otherwise exclude and I am storing in a new

data frame that is zomato\_ratings. After that I am picking values from only Aggregate rating column

and storing it to ratings. Just to make sure there is no nan values





**Plot the bar graph top 10 restaurants in the data with the highest number of votes.**

I used the function sort values on the basis of number of votes. And finally plotted the result.

**Plot the pie graph of top 10 cuisines present in restaurants in the USA**

To tackle empty values i used fillna and during the computation part skipped it . I filtered the data on

the basis of country USA and splitted the data in cuisines by comma and append the data in a list.

Then converted the list ot a pandas series and applied value counts on it to get most frequent

cuisines.





**Plot the bubble graph of a number of Restaurants present in the city of India and keeping the**

**weighted restaurant rating of the city in a bubble.**

As we need to store the city weighted restaurant rating so I am making one city dictionary which will

help me get the city names and the weighted ratings. I have used the same formula which have

been mentioned in one of the previous question to find out the. But here I need to keep track of the

count of restaurant present in the city so I am maintaining that by updating the count by one

whenever I encounter the same city name. So basically here key is city and value is the list wherein

0th storing the summation of votes\*ratings, 1st column storing the summation of votes and 2nd

column storing the count of restaurants present in that city. Once I got the dictionary filled with values

I have calculated the weighted rating and stored in a list named city\_ratings with city name and total

count. after that I have sorted based on the count of restaurants present in the city. So number of

cities can be huge so I have considered top 20 cities in India. Delhi topped among the of cities. After

that I have plotted them in the graph and provided the size of the bubble based on the weighted

rating of the city.





