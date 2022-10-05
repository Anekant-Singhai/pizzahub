# Backend Login Form
NOTE FOR THE DEVELOPERS:


 I made the index , login and register forms different , also there's a ".alert" box in the CSS file , it's important , please don't remove , add as much you need , but before removing look out if that particular thing is being used in back-end or not
while chaning the front-end files content: please look that those elements are not being used in : form.js,server.js,home.js
PS: Once you clone it make sure you run 'npm install' command to install all libraries mention in package.json file.



FOR DATABASE:
there's a database called the "pizzahub" if you want to run this in your machine , please create the database first:
	step1- go to postgres user by giving the command:
		psql -U postgres
	step2 - CREATE DATABASE pizzahub
	step3 - copy this in the terminal as it is:

CREATE TABLE users (id serial not null primary key, name varchar(255) not null, email varchar(255) not null unique, password varchar(255) not null);
	
	step4 - open the server.js file , and give the password for the postgres user in the line 11 which says password under the db section , so that the site can update the users table	
	step4 - go to the folder where the server.js file is stored and give the command: node server.js
and it'll start on port: 3000




