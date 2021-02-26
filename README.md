# Udacity Data Engineer Course / Project 2: Data Modeling with Cassandra
## 1 Description
A startup called Sparkify have been collecting data on songs and user activity on their new music streaming app. The data reside in a directory of CSV files on user activity on the app. To analyze the data in case of what songs users are listening to, this project implements an ETL Pipeline to pre-process the CSV files, save the data one CSV file and afterwards the data of the CSV file is saved in different tables inside an Apacha Cassandra database.

## 2 Queries
The tables are created for the following queries:
1. Give me the artist, song title and song's length in the music app history that was heard during sessionId = 338, and itemInSession = 4
2. Give me only the following: name of artist, song (sorted by itemInSession) and user (first and last name) for userid = 10, sessionid = 182
3. Give me every user name (first and last) in my music app history who listened to the song 'All Hands Against His Own'

## 3 Project Setup
### 3.1 Prerequisites
The following tools/packages/frameworks have to be installed on your system
- docker and docker-compose
- jupyter (to open the jupyter notebook) and inside cassandra-driver and pandas

### 3.2 Run the project
- First run ```docker-compose up``` to fire up the Apacha Cassandra db

Jupyter Notebook:
1. Project_1B_ Project_Template: run all commands inside the Project_1B_ Project_Template.ipynb. This will pre-process the CSV files and save the data one CSV file. It will also create a cluster, keyspace and different tables for the queries and the data of the CSV file is saved in the tables inside the Apacha Cassandra database.


## 4 Jupyter Notebooks
| Name                      	    | Description                                                    	|
|---------------------------------- |----------------------------------------------------------------	|
|Project_1B_ Project_Template.ipynb | Pre-process CSV files, save one events CSV file, creates cluster, keyspace, tables and fills the table with the data from the CSV file |