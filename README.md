<img alt="taxi-service logo" src="/.github/taxi-service-logo.jpg" />

# taxi-service
:oncoming_taxi:  :oncoming_taxi:

> You can see working version in:
> https://my-test-taxi-service.herokuapp.com/index

## :taxi: Description of project
This service is designed to facilitate control over drivers and taxi fleet in your service.
This service is written as a web application, in order to make remote access to the database more convenient.

Thanks to this service, you can control all your cars, all your drivers and assign their cars to drivers,
and all this through the browser interface.
Only users registered in the system have access to the database. Log in using a username and password

## :books: Project structure

| Tier        | Description                              |
|-------------|------------------------------------------|
| JSP-pages   | Response for UI                          |
| Filter      | Response for filtering not-logging users |
| Controllers | Response for controlling HTTP methods    |
| Services    | Response for precessing data             |
| DAO         | Response for connection with DB          |


## :globe_with_meridians: Technologies

- JAVA
- Java Servlets
- JDBC
- Dependency Injection
- JSP
- HTTP(GET, POST, Filters)
- TomCat
- MySQL
- Maven

# інструкції по запуску проекту(обовʼязково)
## :mate: How to start project
### First of all try go to the link and try my demo.
If you can't enter by you login, try to register 
by adding driver.
By this way you can see how look ui.

### On you computer:
- First of all you need initialize database.
Go to:
> /srs/main/resources/init_db.sql

And copy-past it in you database query. 
I recommend use MySql.

- Configure properties of connection to DB
Go to:
> /srs/main/java/taxi/util/ConnectionUtil.java

And set fields url to you database, with port.
And set username and password to you connection.

- Build war file
In console, when you in the root folder run command
> mvn package

After this you need to run this on server.
You can use tomcat, or every server what you like.
