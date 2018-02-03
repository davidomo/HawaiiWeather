# HawaiiWeather

A quick look at the weather patterns of Hawaii using Python and SQL Alchemy.

The goal of this project was to find an ideal time to plan a visit to Hawaii where the temperature is just right and the rain won't get in the way. Looking at percipitation and temperature readouts from different weather stations along the islands, this package will help you plan a trip by looking at past trends.

The project started with two CSV files (Resources/hawaii_measurements & Resources/hawaii_stations) with some basic weather data. File "data_engineering" is using Python Pandas to read in the CSV data to clean and reformat the data. Files in the Resource folder entitled "clean_" denote the ready-to-use files. From there, the data is read into and created into a SQLite database ("hawaii.sqlite) through scripts in file "database_engineering". Modular classes are constructed and the CSVs were added to this local SQL database for queries.

SQL queries are used via Python scripts. Some of these query outputs are visualized as graphs in the "Figures" folder.

Additionally, an API can be made locally using Python and Flask. Locally these APIs can display either the entire history from the database for a specific topic or they can be dynamiclly coded to find temperature data from a date range.
