# cinema-app
![view_img](https://i.paste.pics/84e7f502882625adc631a06cb8b1e044.png)

This is simple cinema-app service with REST API, where you
can buy tickets as user. Also, you can add movies, dates 
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

TIPS: all data store at relative DB. All sensitive data are 
stored in hashed form.

#### List of endpoints:
* PERMIT FOR ALL
  * ../register
  * ../login
* ONLY FOR ADMIN AND USER (HttpMethod.GET):
  * ../cinema-halls/
  * ../movies/
  * ../movie-sessions/available 
* ONLY FOR ADMIN (HttpMethod.GET, POST, PUT, DELETE):
  * ../users/by-email
  * ../cinema-halls/
  * ../movies/
  * ../movie-sessions/
  * ../movie-sessions/{id}
* ONLY FOR USER (HttpMethod.GET, POST, PUT)
  * ../orders/
  * ../shopping-carts/by-user
  * ../orders/complete
  * ../shopping-carts/movie-sessions

## :electric_plug: Technologies
* [X] JDK 17
* [X] Maven 3.8.1
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
    * use [db.properties](https://github.com/apc10bbe/cinema-app/blob/main/src/main/resources/db.properties) to connect to your DB
    * change URL to yours
    * change USERNAME to yours
    * change PASSWORD to yours
    * change JDBC DRIVER to yours
5. Install [Tomcat 9.0.50/9.0.69](https://tomcat.apache.org/download-90.cgi)
6. Setup configurations on Tomcat and run application

TIPS: You already have one administrator account with login
```admin@gmail.com``` and password ```admin``` or you can 
change it at [DataInitializer](https://github.com/apc10bbe/cinema-app/blob/main/src/main/java/cinema/config/DataInitializer.java).


