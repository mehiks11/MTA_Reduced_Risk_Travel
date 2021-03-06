## Guide for Reduced Risk Travel Through the NYC Subway System

### Abstract

The goal of this project was to use visualizations to depict best times and stations for low risk travel during the COVID-19 Pandemic for at-risk populations in New York City. I worked with turnstile data directly provided by the MTA, along with two other data sets that provided ADA accessibility information, as well as geolocational information. Leveraging these three data sets helped me build an interactive map within the code jupyter notebook that allows you to compare average traffic levels between stations on various days of the week. This graphic is supplemented and generally aided by heatmap visualizations, which provide a more in-depth look at traffic levels during certain times of the day and week. These results could greatly aid immunocompromised and older travelers in deciding when to plan certain trips around the city. 

### Design

This project draws its main data from the Metropolitan Transportation Authority of NYC. The final results provide an analysis of traffic levels at different times, comparable between stations around the city. This data will help guide at risk travelers away from peak travel hours, and help guide decisions on planning for travel. Additionally, there is a specific look at ADA accessible stations for people with disabilities. 

### Data

This dataset contains 2,365,405 entry points for various hours of various turnstiles in all the provided stations and divisions. Analysis is mostly broken up by station and division. Each entry point has several features, of which entries, exits, longitude, latitude, station, division, date and time are the most important to this project. Exits and entries were used to determine activity levels while other features were used for plotting purposes or grouping purposes.

### Algorithms

This project involved creating an activity column to determine traffic levels. From here, ranking was done to garner the top ten most travelled stations to determine general trends in these locations. Additionally, the same was done for the top ten most travelled ADA accessible stations, which only differed by some small number of stations.


### Tools
* Numpy and pandas for data manipulation and cleaning
* Seaborn and matplotlib for visualizations
* Bokeh for mapping visualization


### Communication 

Both the slides and visuals will be a part of my communication efforts for this project. Ideally, I would like to add an accessible way to look through the interactive map located in the jupyter notebook.

-------- 

This project utilizes [MTA public turnstile data](http://web.mta.info/developers/turnstile.html "MTA Turnstile Data") to guide immunocompromised transit riders to safer travel times/locations during COVID. The project garners flat data from the [last three months](https://github.com/mehiks11/Metis_MTA_Project/tree/master/data "MTA Project Weekly Flat Data Sets") to rank times, stations, and lines by traffic. [This notebook](https://github.com/mehiks11/Metis_MTA_Project/blob/master/Metis_MTA_Project_Code.ipynb "MTA Project Notebook") details the process of data cleaning and final results production for the project.

The original project proposal with initially set intentions and goals for the project can be found [here](https://github.com/mehiks11/Metis_MTA_Project/blob/master/Project%20Proposal.ipynb "Project Proposal").


### **Data:**

[Here](https://github.com/mehiks11/Metis_MTA_Project/blob/master/mta.db "MTA SQL Database") is the merged database with the three months of data that was queried into python via SQLAlchemy. 

[Here](http://web.mta.info/developers/data/nyct/subway/Stations.csv "MTA ADA Accessibility Data") is another data set with ADA accesibility information, as well as geographic data that can be used for geographic mapping and interactive plotting. 

[Here](https://qri.cloud/nyc-transit-data/remote_complex_lookupcsv "MTA Complex ID Data") is another data set used to combine the above two data sets. It contains complex ID information. 
