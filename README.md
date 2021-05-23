# Bike_Sharing

### Purpose

The purpose of this analysis is to provide compelling input for a business investment proposal for a bike-sharing program in Des Moines, Iowa.  The basis for this analysis will be ride-sharing data from the New York City CitiBike ride sharing program.  

Using publicly available data from the CitiBike website the analysis will be presented using Tableau visualizations along with Pandas to assist in reformatting some key data.

The Tableau story book for this analysis can be viewed via the following link:

[CitiRideAnalysis](https://public.tableau.com/profile/bob.ciminera#!/vizhome/CitiBike_bikesharing/CitiRideAnalysisStory)


### Results

There were two major steps to the analysis.  The first was to extract, transform, and load the citBike data to Tableau and teh second was to create a set of Tableau visualizations to suport the business case

### I. Change "tripduration" to date time format

The  201908-citibike-tripdata.csv.zip file was downloaded from the citiBike website and used as the basis file.  Using Pandas in Jupyter Notebook the tripduration field in the file was transformed from an integer into a date field using the datetime function in pandas.

The following data frame was created and then loaded into a csv file without: 

<img src="https://github.com/rciminera/Bike_Sharing/blob/main/Screen_Shots/citibike_tripdata_df.png" width = "800" >


### II. Create Visualizations

To demonstrate to investors the background behind the bike sharing business plan. A set of Tableau visualizations was created from the citiBike dataset.  Examples of these are below

1. Checkout Times for All Users

This visualization shows that the majority of bikes are checked out for 22 minutes or less with a long tail after 30 minutes.

<img src="https://github.com/rciminera/Bike_Sharing/blob/main/Checkout_Times_for_Users.png" width = "800" >

2. Checkout Times for All Users by Gender

Males represent the majority of riders, however, there is little difference in the amount of time that bikes are checked out between males and females.

<img src="https://github.com/rciminera/Bike_Sharing/blob/main/Screen_Shots/Checkout_Times_for_Users.png" width = "800" >


3. Trips by Weekday per Hour

The hours of highest ridership during weekdays are 7AM to 10AM and 5PM to 8PM.  On Saturdays and Sundays the peak hours are between 10AM and 8PM.

<img src="https://github.com/rciminera/Bike_Sharing/blob/main/Screen_Shots/Trips_by_Weekday_per_Hour.png" width = "800" >


4. Trips by Weekday per Hour by Gender

While there are significantly more Male then Female riders, patterns of peak riding times do not differ between genders.

<img src="https://github.com/rciminera/Bike_Sharing/blob/main/Screen_Shots/Trips_by_Gender_Weekday_per_Hour.png" width = "800" >


5. Trips by Gender by Weekday

Startimes for Customer ridership are highest on Saturday and Sundays whereas Subscriber ridership is highest during the week with Thursday representing the highest.

There appears to be no significant difference in start times  between Genders.

<img src="https://github.com/rciminera/Bike_Sharing/blob/main/Screen_Shots/User_Trips_by_Gender_by_Weekday.png" width = "800" >

6.  Customers

Customers can be grouped into two categories: Subscribers and Customers.  Subscirbers are pre-registered frequent users and customers are transient users such as tourists.  The majority of riders are subscribers.

<img src="https://github.com/rciminera/Bike_Sharing/blob/main/Screen_Shots/customers.png" width = "800" >


7.  Top Ending Locations

There are clusters of high volume activity in specific drop off points.  Knowing what these are can assist in building a similar pattern for DesMoines to make sure that bikes are available to get to these points.

<img src="hhttps://github.com/rciminera/Bike_Sharing/blob/main/Screen_Shots/Top_ending_locations.png" width = "800" >



### Summary 

Even though DesMoines, Ia. is a much different city than New York City, many insights can be applied from the analysis of the New York data.  The lessons learned about timing, ride duration, gender use, pickup and drop off locations among other things can be applied to the Des Moines program.

Two additional visualizations that would provide useful to the business plan would include:

1. Analysis of the top 10 drop off and pick up locations in NYC.
2. Analysis of drop off and pick up location pairs.

In conclusion, the team in DesMoines can build a solid business plan from the analysis of the NYC citiBike ride sharing program.




