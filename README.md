# Project_3308
Main Project Repository for 3308


Repo Structure:
This repo consist of code for our CSCI 3308 Project.  In this repo you can find source code for our project in two formats:
1. Local
2. Heroku

If you would like to run the project locally, then clone or download the 'local' folder and then follow the instructions below:

1. Initialize the login databse:
1a).
sudo -u postgres psql

1b).
create database login_db;

1c).
\c login_db;

1d). 
/* Create the tables */

CREATE TABLE IF NOT EXISTS users(
  id SERIAL PRIMARY KEY,           /* Unique identifier for each user */
  username VARCHAR(50) NOT NULL,   /* The user's login name */
  password VARCHAR(50) NOT NULL);  /* The user's password */


1e).
/* Insert data into tables */

INSERT INTO users(username, password)
VALUES('user1', 'crypto1'); /* samle user login credentials */

2. Start the project:
//Open a terminal in the backend folder and execute the following commands
2a). node index.js

2b). Open the home page in localhost3000/home

