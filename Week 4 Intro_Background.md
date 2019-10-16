# Anaylyzing Comics and Games stores.
#### by H Victor
#### October 16, 2019

### 1. Introduction
#### 1.1 Background
Comics and Games stores are on the rise.  The ability to provide a great environment for likeminded people to meet and play their favorite table top game or read a comic book.  Games like Dungeons & Dragons or Warhammer are great to build upon ones creative and imaginative strategy building gamer minds.  Finding places like this are sometimes quite tough to do.  As finding stores that do one but not the other may occur.  Or the location may just not be in reach. These environments are great for the community.  

#### 1.2 Problem
Why aren't there more of these types of stores in larger cities?  The aim of this project is to help potential investors learn about the location\environment for Comics and Games stores in major cities.  Hoping to help them identify what type of environment would be of interest when predicting their next investment opportunity in building out a Comics and Games store.  

#### 1.3 Interest
Large collectors with investment capital with the passion of wanting to expand their portfolio of investing in brick and mortar shops.  Surrounding their passion for comic books and table top games!


### 2. Data

#### 2.1 Data Sources

* Foursquare API [1]
* Geopy Geocoders [2]

#### 2.2 Why these data sources?

By leveraging the API from Foursquare a search for "Comic's and Games" will return results based on a set size and amount to be returned.  Of course, a location is also needed to help narrow the search.  This is where Geopy comes in.  By combining Geopy with a city and state it will return a location within the form of longitude and latitude.  With this location data a narrowed search will then be performed on the "Comic's and Games" search string within the Foursquare API.  With that location data we can then leverage Foursquares API to return important information about the surrounding venues.  Potentially leading to insights to help predict areas that would provide a suitable location for a new Comic's and Games business.

#### 2.3 Data Source Caveats

Being that this project is a smaller version of what would encompass a larger initiative.  This project will be focusing on data based on the following search criteria: "Comic's and Games".

It is to be noted that additional search criteria would need to be included for future iterations.  Which will need to include a deeper filtering analysis since words like "Hobby" or "Comic Shop" could potentially be meant to mean the same thing as "Comic's and Games".  However, both "Hobby" and "Comic Shop" may not be in the same realm as what we are looking for.  As searches for "Hobby" leads to craft stores or remote-control car's\airplanes businesses.  Then for "Comic Shop" there is a potential that the business is only geared for comic books and table top games will not be available at the store.  

For the purposes of this project the only search criteria that will be used via FourSquares API will be "Comic's and Games".  This will open a peek inside the potential of data science and what it can achieve. 

+Note: Leaving this section open as further development may come to light as this project progresses along.

### 10. References:

1. https://foursquare.com
2. https://geopy.readthedocs.io/en/stable/
