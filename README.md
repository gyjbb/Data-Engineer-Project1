# Data-Engineer-Project1
Sparkify song datasets ETL

## Project Objective

The purpose of this project is to help the startup Sparkify to analyze the activity and song data, which is collect on a daily basis from the app users, and finally to improve the app's user experience. All the datasets are in JSON logs and is not convenient for further queries. So data database schema and ETL pipelines are built in this program to proccess files into tables, benifiting the further analysis of the data collected.


## Instructions on how to run Python script

For .ipython and .py files, it is easy to run in the Jupyter Notebook environment.
create_tables.py and etl.py have to be run before the final sanity test. And the process of running them is already included in the final sanity test file. So Just need to click "Restart and run the kernel" in the test.ipython file.
sql_queries.py includes all the queries needed for the project and is completed.


## Explanations for the files

test.ipython file helps to check the database created and do the sanity test for checking possible errors in data type and table constrains.
create_tables.py file connects to the cursor, drop and create tables.
etl.ipython file reads and processes a single file from the datasets and contain instructions on the ETL process.
etl.py file reads and processes all the files from the datasets, and create the final table.
sql_queries.py contains all the sql queries used in the project.

![songplay table](https://github.com/gyjbb/Data-Engineer-Project1/blob/main/songplay_table.png?raw=true)
