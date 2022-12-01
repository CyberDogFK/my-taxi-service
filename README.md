<img alt="taxi-service logo" src="/.github/taxi-service-logo.jpg" />

# taxi-service
:oncoming_taxi:  :oncoming_taxi:

> You can see the working version in the:
> https://my-test-taxi-service.herokuapp.com/index

## :taxi: Description of project
This service is designed to facilitate control over drivers and taxi fleets in your service.
This service is written as a web application, to make remote access to the database more convenient.

Thanks to this service, you can control all your cars, and all your drivers and assign their cars to drivers,
and all this through the browser interface.
Only users registered in the system have access to the database. Log in using a username and password
When i create this project for depencency injectoin 

## :books: Project structure

| Tier                | Description                                 |
|---------------------|---------------------------------------------|
| JSP-pages           | Responsible for UI                          |
| Filter              | Responsible for filtering not-logging users |
| Controllers         | Responsible for controlling HTTP methods    |
| Services            | Responsible for processing data             |
| DAO                 | Responsible for connection with DB          |
| Dependency Injector | Responsible for dependency inversion        |


## :globe_with_meridians: Technologies

- JAVA 11
- Java Servlets
- JDBC
- JSP
- TomCat 9
- MySQL 8
- Maven 3

## :mate: How to start the project
### First of all try to go to the link and try my demo.
If you can't enter by your login, try to register
by adding a driver.
In this way, you can see how look UI.

### On your computer:
- First of all, you need to initialize the database.
  Go to:
> /srs/main/resources/init_db.sql

And copy-paste it into your database query.
I recommend using MySql.

- Configure properties of the connection to DB
  Go to:
> /srs/main/java/taxi/util/ConnectionUtil.java

And set the field URL to your database, with port.
And set a username and password to your connection.

- Build a war file
  In the console, when you are in the root folder run command
> mvn package

After this, you need to run this on the server.
You can use tomcat, or any server that you like.
