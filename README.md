1.Discuss the purpose of this database in the context of the startup, Sparkify, and their analytical goals.

the purpose of this database is analysis the data it've been collecting on songs and user activity on their new music streaming app and analyze to understand what songs users are listening.


2.State and justify your database schema design and ETL pipeline.

a) database schema design

In my understanding, Database schema design is collecting data into a Dimensional Model schema
This makes the data ready to be analyzed and how are those data related.  

Example 

songplays contains songplay_id, start_time, user_id, level, song_id, artist_id, session_id, location, user_agent. songs contains song_id, title, artist_id, year, duration 

When create dimention table, we should separate the users into another table because the user table doesn't need to keep the song_id.Beside,you must create fact table for connecting relation in each table(dimention) 


b)ETL pipeline

In my understanding, ETL pipeline easy to use when the team want to use data for analysis.You can select extracted data to run queries and compare your results with your expected results.So Postgres has datatypes that probably would easier to match data and faster to use in queries.

