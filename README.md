## MTA Project-- Guide for Reduced Risk Travel Through the NYC Subway System


This project utilizes [MTA public turnstile data](http://web.mta.info/developers/turnstile.html "MTA Turnstile Data") to guide immunocompromised transit riders to safer travel times/locations during COVID. The project garners flat data from the [last three months](https://github.com/mehiks11/Metis_MTA_Project/tree/master/data "MTA Project Weekly Flat Data Sets") to rank times, stations, and lines by traffic. [This notebook](https://github.com/mehiks11/Metis_MTA_Project/blob/master/Metis_MTA_Project_Code.ipynb "MTA Project Notebook") details the process of data cleaning and final results production for the project.

The original project proposal with initially set intentions and goals for the project can be found [here](https://github.com/mehiks11/Metis_MTA_Project/blob/master/Project%20Proposal.ipynb "Project Proposal").


###**Data:**

[Here](https://github.com/mehiks11/Metis_MTA_Project/blob/master/mta.db "MTA SQL Database") is the merged database with the three months of data that was queried into python via SQLAlchemy. 

[Here](http://web.mta.info/developers/data/nyct/subway/Stations.csv "MTA ADA Accessibility Data") is another data set with ADA accesibility information, as well as geographic data that can be used for geographic mapping and interactive plotting. 

[Here](https://qri.cloud/nyc-transit-data/remote_complex_lookupcsv "MTA Complex ID Data") is another data set used to combine the above two data sets. It contains complex ID information. 
