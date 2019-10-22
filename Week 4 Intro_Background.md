# Anaylyzing Comics and Games stores.
#### by H Victor
#### October 16, 2019

### 1. Introduction
#### 1.1 Background
I believe Comics and Games stores are on the rise.  The ability to provide a great environment for likeminded people to meet and play their favorite table top game or read a comic book has been brought up in a number of conversations amongst peers.  Games like Dungeons & Dragons or Warhammer are great to build upon ones creative and imaginative strategy building gamer minds.  It seems that there are not as many of these types of establishments as there should be.  As finding stores that do one but not the other may occur or the location of a store may just not be in reach. 

#### 1.2 Problem
Why aren't there more of these types of stores in larger cities?  The aim of this project is to help potential investors learn about the area around Comics and Games stores, found from Foursquare's API, in a select number of cities.  Hoping to help shed some insight in identifying the type of environment surrounding Comics and Games stores as gathered from FourSquare.  I believe this will be of interest for when an invester is looking to predict their next investment opportunity in building out a Comics and Games store.  

#### 1.3 Interest
Large collectors with investment capital with the passion of wanting to expand their portfolio of investing in brick and mortar shops.  Surrounding their passion for comic books and table top games!  These environments create a great atmosphere for the community to meet and build frienships with people who share in similar interests. 


### 2. Data

#### 2.1 Data Sources

* Foursquare API [1]
* Geopy Geocoders [2]

#### 2.2 Why these data sources?

By leveraging the API from Foursquare a search for "Comic's and Games" will return results based on a set size and amount to be returned.  Of course, a location is also needed to help narrow the search.  This is where Geopy comes in.  By combining Geopy with a city and state it will return the cities longitude and latitude.  With this location data for the city a search will then be performed using a "Comic's and Games" search string within the Foursquare API.  With the returned coordinates from the previous search from Foursquare we can then leverage Foursquares API to return insight into the surrounding venues around these stores.  Potentially leading to insights in the surrounding areas that could lead to ideas for a suitable location for a new Comic's and Games business.  By levereaging K-means clustering we can group similar environments together together based on the types of venues in the area.

#### 2.3 Data Source Caveats and Cleaning

Being that this project is a smaller version of what would encompass a larger initiative.  This project will be focusing on data based on the following search criteria: "Comic's and Games" from Foursquares API.  

It is to be noted that additional search criteria would need to be included for future iterations.  Which will need to include a deeper filtering analysis since words like "Hobby" or "Comic Shop" could potentially be meant to mean the same thing as "Comic's and Games".  However, both "Hobby" and "Comic Shop" may not be in the same realm as what we are looking for.  As searches for "Hobby" leads to craft stores or remote-control car's\airplanes businesses.  Then for "Comic Shop" there is a potential that the business is only geared for comic books and table top games will not be available at the store.  

For the purposes of this project the only search criteria that will be used via FourSquares API will be "Comic's and Games".  This will open a peek inside the potential of data science and what it can achieve. In addition to this we will be filtering out any shops that do not run a category of "Comic Shop".  

It has been identified that duplicate entries for a business may be returned under the initial search.  To help stream line the use of data.  Any business that looks like a duplicate will be removed from the intial data set.  

+Note: Leaving this section open as further development may come to light as this project progresses along.

### 2.4 Data Search Varaibles

Geopy:  This module is able to return the longitude and latitude for a city and state.  Here is a list of cities and the state that will be used.
1. Fort Worth, TX
2. San Antonio, TX
3. Austin, TX
4. Houston, TX

### 10. References:

1. https://foursquare.com
2. https://geopy.readthedocs.io/en/stable/
