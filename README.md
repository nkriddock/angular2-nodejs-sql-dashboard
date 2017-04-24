# Angular2,NodeJs and Sql Dashboard

Basic Dashboard feature list:

 * Angular Material Design
 * Bootstrap3
 * D3 Visualization
 * Font Awesome
 * Teradata UI Platform

 ## Usage

  * ### Step 1
  ```
  CREATE DATABASE <DB Name>;

  Example:   CREATE DATABASE personDB;

  USE <DB Name>

  Example: USE personDB

  CREATE TABLE `personslist` (
    `PersonID` int(11) NOT NULL AUTO_INCREMENT,
    `LastName` varchar(255) NOT NULL,
    `FirstName` varchar(255) NOT NULL,
    `Address` varchar(255) NOT NULL,
    `City` varchar(255) NOT NULL,
    PRIMARY KEY (`PersonID`)
  ) ENGINE=InnoDB AUTO_INCREMENT=114 DEFAULT CHARSET=utf8;


  ```
* ### Step 2
 configuration setup nodeJS
 ```
 cd setup-nodejs-server-with-sql-database
 ```
  ```
       Edit in Server.js
       var connection = mysql.createConnection({
           host: '<host>',
           user: '<user>',
           password: '<password>',
           database: '<DB Name>'
       });
       if you want to change port

       app.listen(<port number>);
       Example :   app.listen(4442);

        ```
        Install package.json dependencies
setup-nodejs-server-with-sql-database> npm install
         ```
           ```
                 Run Node Server
         setup-nodejs-server-with-sql-database>Node Server

         Go to url:

         http://localhost:4442/app
                  ```