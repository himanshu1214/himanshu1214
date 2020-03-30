# About Project:
The project is concerned with creating Dimensional and Fact Tables using songs and 
log tables. Further ETL of data into postgres was accomplished. The project consist of 
create_table.py, sql_queries.py and etl.py. 

# About Data:
### Logs_Data: 
##### Soure: https://github.com/Interana/eventsim
##### Variables: artist	auth	firstName	gender	itemInSession	lastName	length	level	location	method	page	registration	sessionId	song	status	ts	userAgent	userId
### Songs_Data:
##### Source: http://millionsongdataset.com/
##### Variables: artist_id	artist_latitude	artist_location	artist_longitude	artist_name	duration	num_songs	song_id	title	year
    
  
# Modules:
#### etl.py - 
get the json log, song files and populates the dimensions and fact tables on postgres database

#### sql_queries.py - 
Queries to create Dimension and Fact tables, insert data and drop tables

#### create_table.py - 
Queries to create the database on postgres and run the sql queries, populate the database 
with tables .
Dimension Tab - users Table : user_id, first_name, last_name, gender, level 
                songs Table : song_id, title, artist_id, year, duration
                time Table : start_time, hour, day, week, month, year, weekday
                artists Table : artist_id, name, location, latitude, longitude
                
Fact Table: songplay Table: songplay_id, start_time, user_id, level, song_id, artist_id, session_id, location, user_agent
#### RESULT  
POPULATED THE DATA 