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

#### 2.2 Why these datasources?

By leveraging the API from Foursquare a search for "Comic's and Games" will return results based on a set size and amount to be returned.  Of course a location is also needed to help narrow the search.  This is where Geopy comes in.  By combining Geopy with a city and state it will return a location within the form of longitude and latitude.  With this location data a narrowed search will then be performed on the "Comic's and Games" search string within the Foursquare API.  With that location data we can then leverage Foursquares API to return important information about the surrounding venues.  Potentially leading to insights to help predict what would be 

### 10. References:

1. https://foursquare.com
2. https://geopy.readthedocs.io/en/stable/
