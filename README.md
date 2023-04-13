# Python-API-Challenge

WeatherPy

To start the WeatherPy part of this assigment I used the starter code given to me and use the code to generate a number of cities. I then put these cities in an empty list so that I can retrive the weather data for each city. I then used the JSON to retrieve the data. Within the data I fouces on the data elements of latitude, longitude, max temp, humidity, cloudiness, wind speed, country, and date. I then appended those data elements into the empty list of cities I created. This gets it so that I have all this data for each city in the list. After I ran the code the cities that didn't have any data got dropped from the list. So I lost a few cities after I ran the code. 

Then I showed the data table of all the cities I have in the list. The tabel is below: 

  <img width="782" alt="Screenshot 2023-04-13 at 11 40 01 AM" src="https://user-images.githubusercontent.com/125215083/231827512-52580418-3eb2-4c2d-bd01-cdb7762d0931.png">

I then converted this data set into a CSV file and exported it so that it could be used in the VactionPy part of the assignment. 

Then to get ready for the graphing section I pulled out all the relevant data that would be used for the scatter plots. This includes latitude, max temp, humidity, cloudiness, and wind speed. 

The first scatter plot I created was for latitude vs. temperature. The scatter plot is below: 

  <img width="427" alt="Screenshot 2023-04-13 at 11 44 01 AM" src="https://user-images.githubusercontent.com/125215083/231828372-72dbdfde-da05-484f-8166-e73e12d68ab0.png">

The second scatter plot I created was for latitude vs. humidity. The scatter plot is below: 

  <img width="422" alt="Screenshot 2023-04-13 at 11 45 24 AM" src="https://user-images.githubusercontent.com/125215083/231828679-241238b5-953c-4c64-9298-cbe129e18ff9.png">

The third scatter plot I created was for latitude vs. cloudiness. The scatter plot is below:

  <img width="417" alt="Screenshot 2023-04-13 at 11 46 47 AM" src="https://user-images.githubusercontent.com/125215083/231829096-59f5027f-e218-483d-9d3c-d02e1a1b0e8f.png">

The fourth scatter plot I created was for latitude vs. wind speed. The scatter plot is below: 

  <img width="401" alt="Screenshot 2023-04-13 at 11 48 41 AM" src="https://user-images.githubusercontent.com/125215083/231829621-56dbf4d4-d569-479a-a9bc-ef826411cf69.png">

Then once I was done with all the scatter plots I started to create my linear regression function for the following graphs I create. I also split the data into the northern hemisphere and the southern hemisphere. The northern hemisphere is for latitudes greater than or equal to 0 and the southern hemisphere is for latitudes less than 0. 

There first regression plot is for temperature vs latitude. The northern hemisphere plot is below: 

  <img width="425" alt="Screenshot 2023-04-13 at 11 59 23 AM" src="https://user-images.githubusercontent.com/125215083/231831920-8707b206-1268-4f90-86c4-dfc7694833f4.png">

The plot for the southern hemisphere is below: 

  <img width="424" alt="Screenshot 2023-04-13 at 12 00 52 PM" src="https://user-images.githubusercontent.com/125215083/231832257-4eebc5f8-4d12-40b0-94cd-60dc922eb2c6.png">

My response to these graphs is that there is a large positive correlation between temperature and latitude in the northern hemisphere. There is also a large positive correlation between temperature and latitude in the southern hemisphere. This would make sense becasue the equator splits the northern and southern hemispheres of the earth. It is also warmer near the equator which is shown in both graphs, at 0 latitude the temperatures are at their highest. Then as the latitude moves away from 0, the temperatures come down because we are moving away from the equator. 

The second regression plot is for humidity vs latitude. The northern hemisphere plot is below: 

  <img width="403" alt="Screenshot 2023-04-13 at 12 07 32 PM" src="https://user-images.githubusercontent.com/125215083/231833696-96e73a99-2001-43f6-90e0-0095abaa0bd0.png">

The southern hemisphere plot is below: 

  <img width="415" alt="Screenshot 2023-04-13 at 12 08 31 PM" src="https://user-images.githubusercontent.com/125215083/231833974-25ef4bc4-a0cf-4b01-9905-65fd6ee21885.png">

My response to these graphs is that there is a small positive correlation between latitude and humidity in the northern hemisphere. There is also a small positive correlation between latitude and humidity in the southern hemisphere. When looking at the northern hemisphere there really isn't a correlation, the data is all over the chart with no real true correlation. There really isn't one for the southern hemisphere either but you can kind of infer from the data points on the graph that the closer to the equator the more humid it is.

The thrid regression plot is for cloudiness vs latitude. The northern hemisphere plot is below: 

  <img width="401" alt="Screenshot 2023-04-13 at 12 13 25 PM" src="https://user-images.githubusercontent.com/125215083/231834942-5d946081-1514-443e-b510-6f87385ead9e.png">

The southern hemisphere plot is below: 

  <img width="416" alt="Screenshot 2023-04-13 at 12 14 27 PM" src="https://user-images.githubusercontent.com/125215083/231835142-b0a7ad4e-2f3e-4839-9e35-30031d4dfa83.png">

My response to these graphs is that there is a small positive correlation between latitude and cloudiness in the northern hemisphere. There is also a small positive correlation between latitude and cloudiness in the southern hemisphere. When looking at both hemispheres there really is not a true correlation between latitude and cloudiness. This means that one is not related to the other and they do not affect each other.

The last regression plot is for wind speed and latitude. The northern hemisphere plot is below: 

  <img width="403" alt="Screenshot 2023-04-13 at 12 18 32 PM" src="https://user-images.githubusercontent.com/125215083/231835937-35859e18-603e-460f-b3c7-963170605126.png">

The southern hemisphere plot is below: 

  <img width="402" alt="Screenshot 2023-04-13 at 12 19 35 PM" src="https://user-images.githubusercontent.com/125215083/231836131-556ac2e5-446a-4c48-ab49-682e8201e911.png">

My response to these graphs is that there is a pretty small positive correlation between latitude and wind speed in the northern hemisphere. There is a small positive correlation between latitude and wind speed in the southern hemisphere. There really is no correlation between latitude and wind speed in the northern hemisphere because the r-value is so so small. There is a slight correlation you can make between latitude and wind speed in the southern hemisphere. It is small but you can see in the graph that most of the data points are located in one general area and trend in the same direction. It would look like from the graph that wind speeds are lower closer to the equator but again this correlation is small. 

The second part of this assignment is the VactionPy assignment. To begin this portion of the assingment I imported the CSV file which I saved from the WeatherPy portion of the assignment. I then created a map wiht a point for every city in the dataframe and the size of each point is based on the humidity in each city. The map is below: 

  <img width="871" alt="Screenshot 2023-04-13 at 12 34 11 PM" src="https://user-images.githubusercontent.com/125215083/231839384-42f9030e-e86f-4981-b83f-d42cc2fdec9d.png">

Then I narrowed the data down to fit certian criteria. The criteria is that the temperature is lower than 27 degrees but higher than 21 degrees. The wind speed is less than 4.5 m/s. The last one is that there is zero cloudiness. I then dropped any rows with null values and this created my new dataframe. I then created a dataframe for hotels. This dataframe incudes the columns City, Country, Latitude, Longitude, and Humidity from the dataframe I created in the previus step. I also added a new column in the hotel dataframe called Hotel Name. Then I looked for hotels in each city located within 10,000 meters of the coordinates I set. I looped through all the data in the hotel dataframe and found the nearest hotel. I then printed the hotel name in the chart under in the column I created named Hotel Name. This new clean data table is below: 

  <img width="770" alt="Screenshot 2023-04-13 at 12 42 47 PM" src="https://user-images.githubusercontent.com/125215083/231841318-1618850a-5725-4454-b593-f48244872d26.png">

The last step in this assignment was creating a map with some additional information. The points are of each city in the hotel dataframe and the size of each point is based off of the humidity in each city. This map has additional information where if you hover over the point on the map you will see all the information about that point but you will also see the Country and the name of the nearest hotel. This map is below:

  <img width="1076" alt="Screenshot 2023-04-13 at 12 55 57 PM" src="https://user-images.githubusercontent.com/125215083/231844335-fdce9056-8440-4330-abbc-ba7b0bfda2e7.png">

This is everything I did for this assignment. 
