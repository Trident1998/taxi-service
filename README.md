![taxiService](https://user-images.githubusercontent.com/79996912/124107121-97eb4200-da6d-11eb-986b-877b33b00e94.png)


## Introduction
It's small service web application for drivers who can check their own and others cars for improving 
their work time!

## Functions Of App
After login in, user can use following possibilities:
- add new drivers to DB;
- add new car to DB;
- add new manufacturer to DB;  
- register a driver to some car;
- deleted cars from DB;
- deleted drivers from DB;
- deleted manufacturer from DB;
- show current information about cars, drivers and manufacturers.

## Architecture Of App
Current application uses in their structure N-tier architecture and SOLID principles:
- DAO layer is responsible for work with DB. It was built with the JDBC API;
- Service layer is responsible for processing some business logic;
- Controller layer is introduced with Servlets which receives a request from a client and sends a
  response to them. It is presented with JSP page;
- Filter layer is responsible for control access to the service's functionality.

## Current Technologies
- Apache Tomcat - version 9.0.48
- MySQL - version 8.0.22
- JDBC
- Servlet
- JSTL
- JSP
- HTML, CSS

## How To Run This Project
1. Clone this project into your local folder and open the project in an IDE. 
2. Configure Tomcat Server and set up the MySQL RDBMS on your machine.
3. Replicate the database from the project by copying the script from init_db.sql into 
   the MySQL Workbench query editor window.
4. Insert your own MySQL username and login in dbProperties in the ConnectionUtil class.
5. Setup new connection with:
    user: "your username"
    password: "your password"
    url: jdbc:mysql://xxxx:yyyy/kkkk?serverTimezone=UTC , where:
    xxxx - host name,
    yyyy - port,
    kkkk - database name
6. Run a project