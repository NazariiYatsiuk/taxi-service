# Taxi Service 
![images (1)](https://user-images.githubusercontent.com/94574503/161727692-24f3913f-2d2b-45cc-a5a1-8840d3e5e3ab.png)
## Description
This project is a simple Web application, that imitates basic functions of taxi service. It supports user registration, authentication and CRUD operations to work with data base. App is based on N-tier architecture (DAO, Service and Controller tiers).
## Functions:
* Register a new user (add a new driver to DB);
* Add a new car to DB;
* Add a new manufacturer to DB;
* Show a list of all added cars;
* Show a list of all registered drivers;
* Show a list of all added car manufacturers;
* Show a list of all cars, that are linked to authenticated driver;
* Link a specific driver to a specific car (many-to-many relations);
* Delete specific car from DB (implemented soft delete);
* Delete specific manufacturer from DB (implemented soft delete);
* Delete specific driver from DB (implemented soft delete);
## Used technologies:
* Java 17;
* MySQL _v8.0_;
* JDBC;
* Apache Maven;
* Apache Tomcat _v9.0.50_;
* Apache log4j _v2.8.2_;
* Javax Servlet _v4.0.1_;
* JSTL _v1.2_;
* JSP.
## How to use:
1) Install MySQL DBMS.
2) Run SQL scripts from `/src/main/resources/init_db.sql` to create necessary schema and tables.
3) Configure connection to your DB by filling actual URL (**_line 9_**), username (**_line 10_**), password (**_line 11_**) and JDBC driver (**_line 12_**) into `/src/main/java/taxi/util/ConnectionUtil.java`.
4) Configure logger by filling absolute path to your log file instead "ABSOLUTE_PATH" into `/src/main/resources/log4j2.xml` (line 7). Tip: if file doesn`t exist, it will be automatically created.
5) Install and configure Apache Tomcat (**_version 9.x.x recommended_**).
6) Run Tomcat server and explore all features.
