﻿# Cinema app
![waiting](https://i.pinimg.com/736x/1e/80/b5/1e80b5d72209b48ae768747b2a8fae9b.jpg)
## General info
*Simple cinema service with such functions as authorization and authentication.
User, in this application, can have two roles `admin` or `user`.*
## The current functionality of the program
*There are two ready-made users provided for testing this application:*
- *login admin@i.ua with password admin123 and role `admin`*
- *login bob@gmail.com with password bob and role `user`*

#### The admin has access to such endpoints:
* POST: /cinema-halls
* POST: /movies
* POST: /movie-sessions
* PUT: /movie-sessions/{id}
* DELETE: /movie-sessions/{id}
* GET: /users/by-email

#### The user has access to such endpoints:
* POST: /orders/complete
* PUT: /shopping-carts/movie-sessions
* GET: /orders
* GET: /shopping-carts/by-user

#### Endpoints that can be accessed by any logged-in user:
* POST: /register
* GET: /cinema-halls
* GET: /movies
* GET: /movie-sessions/available

## Technologies
*The following technologies were used in the [project](https://github.com/Eugene-exe/cinema_app):*

- [IntelliJ IDEA 2021.2.3 Ultimate](https://www.jetbrains.com/ru-ru/idea/download/#section=windows)
- [Apache Tomcat (v9.0.55)](https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.50/bin/)
- [Maven Checkstyle Plugin](https://maven.apache.org/plugins/maven-checkstyle-plugin/download.cgi)
- [MySQL (v8.0.25)](https://www.mysql.com/downloads/)
- [Spring (Core, WEB, Security)](https://spring.io/)
- [Maven](https://maven.apache.org/download.cgi)
- Hibernate

## How to start cinema service locally:
1. Install and configure Apache Tomcat.
2. Install and configure and create a schema in MySQL.
3. Fork this project.
4. To connect to database in application you need change configuration information
   in the file from `/resources/db.properties` to the ones you specified when installing MySQL.
5. Start the application.
6. After running the application you will be redirected to login page, where you need to sing in.
