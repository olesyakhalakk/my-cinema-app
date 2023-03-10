# **My-cinema-app**

Simple cinema service app that supports authentication, registration and CRUD operations.

## **_Functionality_**

When a person logs in they have one of two roles (ADMIN or USER), which restricts access to certain functionality of the program.

ADMIN can:
* Get/add cinema halls and movies.
* Get available movie sessions and add/update/delete other ones.
* Get users by their emails.

USER can:
* Get cinema halls, movies and available movie sessions.
* Get all orders and complete any of them.
* Get a shopping cart and add tickets for movie sessions to it.

## **_Project structure_**
The project is built by the N-tire architecture principle. It has 3 layers:
1. Presentation (controllers in cinema/controller)
2. Service (cinema/service)
3. Data access (cinema/dao)

## **_Technologies_**
* JDK 11
* Maven 4.0.0
* Tomcat 9.0.65
* MySQL 8.0.22
* Hibernate 6.1.6
* Spring (Spring Core, Spring Web, Spring Security) 5.6.10

## **_How to run the application_**
* Clone this project.
* Make sure you have Tomcat 9.0.65 installed.
* Make sure you use MySQL as a database otherwise you need to change a dependency in pom.xml.
* Edit URL, username, password and JDBC driver in resources/db.properties.
* Edit Tomcat configuration.
* Run mvn clean package in terminal.
* Run the application (the first user with ADMIN role will be created automatically: email - admin@i.ua, password - admin123).