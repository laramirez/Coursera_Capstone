# Coursera_Capstone

"This capstone project course will give you a taste of what data scientists go through in real life when working with data. 

You will learn about location data and different location data providers, such as Foursquare. You will learn how to make RESTful API calls to the Foursquare API to retrieve data about venues in different neighborhoods around the world. You will also learn how to be creative in situations where data are not readily available by scraping web data and parsing HTML code. You will utilize Python and its pandas library to manipulate data, which will help you help you refine your skills for exploring and analyzing data. 

Finally, you will be required to use the Folium library to great maps of geospatial data and to communicate your results and findings."

## 1/ Toronto Neighborhood Clustering

This assignment required to explore and cluster neighborhoods in Toronto.

The list of Toronto postcodes, boroughs and neighborhoods was scrapped on the Toronto Wikipedia page using Beautiful Soup.
https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M

The list of coordinates for each postcode was supplied by the program.
http://cocl.us/Geospatial_data

This information was combined to create a base Folium visualization of the different neighborhoods:

![Screenshot](toronto_post_codes.png)

The Foursquare API was then used to gather the 100 surrounding venues for each postal code, along with venue categories.

Categories were then manually regrouped into bigger groups, which were used as discriminants to cluster neighborhoods together:

![Screenshot](toronto_post_codes_clustered.png)
