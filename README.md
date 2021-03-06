# Project_3308
Main Project Repository for 3308

#### This project consist of a webpage that allows a user to log in, enter a password, and have the password encrypted using an encryption algorithm of the user’s choice. 


## Repo Structure:
This repo consist of code for our CSCI 3308 Project.  In this repo you can find source code for our project in two formats as well as test classes:
1. Local
2. Heroku
3. Cipher Tests (Test Classes)

## Instructions:
If you would like to run the project locally, then clone or download the 'local' folder and then follow the instructions below:

1. Initialize the login databse:

1a).
```
sudo -u postgres psql
```
1b).
```
create database login_db;
```
1c).
```
\c login_db;
```
1d). 
```
CREATE TABLE IF NOT EXISTS users(
  id SERIAL PRIMARY KEY,           
  username VARCHAR(50) NOT NULL,   
  password VARCHAR(50) NOT NULL);  
```

1e).
```
INSERT INTO users(username, password)
VALUES('user1', 'crypto1'); 
```
2. Start the project:

2a). Open a terminal in the backend folder and execute the following commands:
node index.js

2b). Open the home page in localhost3000/home

To run the test classes follow these instructions:

Open the SpecRunner.html file in any web browser. Make sure all the appropriate files exist in the appropriate folders. The following 2 files are essential:

1. src/Encryptor.js contains the actual encryption algorithims.

2. spec/CipherSpec.js contains the various test cases.

To see a final, deployed version of the app, visit heroku: https://crypto13308.herokuapp.com
