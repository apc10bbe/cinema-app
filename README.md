# cinema-app
![view_img](https://w7.pngwing.com/pngs/275/309/png-transparent-cinema-film-popcorn-food-film-poster-clapperboard.png)

This is simple cinema-app service with REST API, where you
can buy tickets as user. Also you can add movies, dates 
of movies, cinema halls as administrator, use CRUD operations
to control and change the data at Database.
In addition, when you use the service, authentication 
and authorization are required for both: the user and 
the administrator.

#### DB Structure
![db_structure_img](https://github.com/mate-academy/hibernate-configuration-hw/raw/master/Hibernate_Cinema_Uml.png)

## :clipboard: Functional possibilities

#### User Features:
* Login/registration before start using
* Possibility to find available movie sessions
* Possibility to issue tickets
* Ability to complete the order and add tickets to cart

#### Admin Features:
* Ability to add movies
* Ability to manage movie sessions
* Ability to add cinema halls
* Manage users at Database

TIPS: all data store at relative DB. All sensitive data is 
stored in hashed form.

## :electric_plug: Technologies
* [X] JDK 17
* [X] Maven 3.8.1
* [X] WAR 3.3.2
* [X] MySQL 8.0.31
* [X] JDBC API
* [X] Hibernate
* [X] Spring Core
* [X] Spring Web
* [X] Spring Security
* [X] Tomcat 9.0.50/9.0.69

## How to run application

1. Create fork at Github
2. Clone the project to your work space
3. Install MySQL 8
4. Create connection to DB
    * use [db.properties]() to connect to your DB
    * change URL to yours
    * change USERNAME to yours
    * change PASSWORD to yours
    * change JDBC DRIVER to yours
5. Install [Tomcat 9.0.50/9.0.69](https://tomcat.apache.org/download-90.cgi)
6. Setup configurations on Tomcat and run application


