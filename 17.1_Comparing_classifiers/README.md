# AI-Coupon-Statistics
## Will a Customer Accept the Coupon?

Goto [prompt.ipynb](prompt.ipynb) for complete Jupyter Notebook.
------

**Context**

Imagine driving through town and a coupon is delivered to your cell phone for a restaraunt near where you are driving. Would you accept that coupon and take a short detour to the restaraunt? Would you accept the coupon but use it on a sunbsequent trip? Would you ignore the coupon entirely? What if the coupon was for a bar instead of a restaraunt? What about a coffee house? Would you accept a bar coupon with a minor passenger in the car? What about if it was just you and your partner in the car? Would weather impact the rate of acceptance? What about the time of day?

Obviously, proximity to the business is a factor on whether the coupon is delivered to the driver or not, but what are the factors that determine whether a driver accepts the coupon once it is delivered to them? How would you determine whether a driver is likely to accept a coupon?

------
**Overview**

The goal of this project is to use what you know about visualizations and probability distributions to distinguish between customers who accepted a driving coupon versus those that did not.

------
**Data**

This data comes to us from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios including the destination, current time, weather, passenger, etc., and then ask the person whether he will accept the coupon if he is the driver. Answers that the user will drive there ‘right away’ or ‘later before the coupon expires’ are labeled as ‘Y = 1’ and answers ‘no, I do not want the coupon’ are labeled as ‘Y = 0’.  There are five different types of coupons -- less expensive restaurants (under \\$20), coffee houses, carry out & take away, bar, and more expensive restaurants (\\$20 - \\$50). 

------
### Data Description
Keep in mind that these values mentioned below are average values.

The attributes of this data set include:
1. User attributes
    -  Gender: male, female
    -  Age: below 21, 21 to 25, 26 to 30, etc.
    -  Marital Status: single, married partner, unmarried partner, or widowed
    -  Number of children: 0, 1, or more than 1
    -  Education: high school, bachelors degree, associates degree, or graduate degree
    -  Occupation: architecture & engineering, business & financial, etc.
    -  Annual income: less than \\$12500, \\$12500 - \\$24999, \\$25000 - \\$37499, etc.
    -  Number of times that he/she goes to a bar: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
    -  Number of times that he/she buys takeaway food: 0, less than 1, 1 to 3, 4 to 8 or greater
    than 8
    -  Number of times that he/she goes to a coffee house: 0, less than 1, 1 to 3, 4 to 8 or
    greater than 8
    -  Number of times that he/she eats at a restaurant with average expense less than \\$20 per
    person: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
    -  Number of times that he/she goes to a bar: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
    

2. Contextual attributes
    - Driving destination: home, work, or no urgent destination
    - Location of user, coupon and destination: we provide a map to show the geographical
    location of the user, destination, and the venue, and we mark the distance between each
    two places with time of driving. The user can see whether the venue is in the same
    direction as the destination.
    - Weather: sunny, rainy, or snowy
    - Temperature: 30F, 55F, or 80F
    - Time: 10AM, 2PM, or 6PM
    - Passenger: alone, partner, kid(s), or friend(s)


3. Coupon attributes
    - time before it expires: 2 hours or one day

------
### Overall Analysis

 - Overall 58% of drivers accept coupons
 - "Bar" Coupons are accepted more during 55º temperature
 - More the bar visits, higher the acceptance of bar coupon (77% acceptance opposed to drivers who have not been i.e. 37%
 - Higher the age and have visited bar, more likly they accept bar coupons
 - Singles accept more coupon than any other marital status
 - `Carry out and take away` has the highest acceptance rate compared to any other coupon type. 2nd is `Restaurant(<20)`.
 - `Coffee House` has th maximum number of data.
 - less than 1% (0.85%) of drivers have provided car/driving details
 - `Unemployed` and `less than 12.5 k` has the 424 records, second is `Computer & Mathematical` earning more than 100k with 352 records
 - `Architecture & Engineering` has highest number of count
 - `Healthcare Support` has the highest acceptance rate with 69.8347% compared to any other job
 - `Retired` job type has highest rejection rate with 54.1414%
 
 ### Next Steps and Recommendations
 - Try to gather more data of car/vehical, that might provide more insights
 - Provide bar coupon based on weather conditions
 - Come up with geo-locations bassed on profession so that coupons are more targeted by driver professions
 - `Restaurant(<20)` has the second highest acceptane rate, provide more of that coupon

------
