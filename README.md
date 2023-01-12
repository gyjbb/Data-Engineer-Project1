# Data-Engineer-Project1
Normalized database design through Star Schema
Sparkify song datasets ETL

### Project Objective

The purpose of this project is to help the startup Sparkify to analyze the users activity in the app, and finally to improve the app's user experience. The datasets are collected on a daily basis from the app users' song play records. All the datasets are in JSON logs and not convenient for further queries. So database star schema and ETL pipelines are built in this project to proccess files into tables, benifiting the further analysis of the data collected.


### Instructions on how to run Python script

For .ipython and .py files, it is easy to run in the Jupyter Notebook environment. \
The two python files **create_tables.py and etl.py** have to be run before the final sanity test. And the process of running them is included in the final sanity test file. So to finish the ETL process,just need to **click "Restart and run the kernel" in the test.ipython file**. \
The file sql_queries.py includes all the queries needed for the project.


### Explanations for the files

**test.ipython** file helps to check the **songplays, users, songs, artists, time tables** created and do the sanity test for possible errors in data types and table constrains. \
**create_tables.py** file connects to the cursor, drop and create the above 5 tables.\
**etl.ipython** file reads and processes a single file from the datasets and serves the creation of final ETL process.\
**etl.py** file reads and processes all the files from the datasets, and insert data to the final 5 tables.\
**sql_queries.py** includes all the sql queries used in the project. 

**Song datasets** have columns for the **songs and artists tables**, such as song_id, artist_id, title, location. **Log datasets** have columns for **user, and time tables**, such as user_id, gender, level, start_time. And **songplays table** has columns from the log datasets, and also includes information matched with the songs and artists table. \
Below are the first 5 rows of the generated **songplays table**. 
![songplays table](https://github.com/gyjbb/Data-Engineer-Project1/blob/main/songplay_table.png?raw=true)
