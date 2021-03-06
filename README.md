# Group
The purpose of this code is to analyze Primary Health Care services in Lagos, Nigeria.
It would assist policy makers in taking human resource management decisions in the state. in terms of deployment and recruitment of health workers.
Its objectives are to:
•	Determine the population and number of Health Workers in each Local Government Area.
•	Assess the population served per Primary Health Care center in each Local Government Area.
•	Determine the population per health worker in each Local Government Area, both as a whole and by categories
•	Map the spatial distribution of Primary Health Care centers in each Local Government Area.
4 datasets were acquired from e sources. These are
1	Coordinates of health care centers from https://data.world
2	Details of Primary health centers and facilities from Lagos state abstract of local government statistics (2015)
3	Map of Lagos state showing local governments from SMART GIS
4	Population of Lagos State per Local Government Area
The following modules were installed in Google Colab, which was the coding environment:
•	Matplotlib- for data visualization
•	Geopandas- for geospatial data analysis
•	Plotly- used for the interactive visualization 

Data Preparation
Some of the data in the datasets where not useful and were dropped. These are the ‘ownership’ and the ‘LL sources’ columns in the health care centers from https://data.world . The number no of incubators, number of cradles and number of cots in the details of Primary Health Centers and Facilities dataset was also dropped. 

The datasets were then merged. The population dataset was merged with the data for the boundary of each Local Government Area. Also, the population dataset was merged with data for primary health centers.

In addition, some of the columns were renamed both to make them shorter or more explanatory. ‘Joint_Count’ was renamed “No_PHC” in the merged dataset.

Finally, for data preparation, additional columns were created. The sum of all health workers for each column was calculated, the ratio of total number health workers to population in each Local Government Area was also calculated.
The concludes with data analysis and visualization.

The following were technologies used for the platform:
•	SQLite3 for database management
•	Flask for creating the server and API
•	Npm node.js
Process
1.	The database was created using SQlite because it is light 
2.	The database was populated
3.	Python server using Flask
4.	APIs were written to return data with python language using flask
5.	The front end was created using react.js


