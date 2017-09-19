1. Create database & table in MySQL first :

CREATE DATABASE IF NOT EXISTS websystique;
USE websystique;

CREATE TABLE EMPLOYEE(
	id INT NOT NULL auto_increment, 
	name VARCHAR(50) NOT NULL,
	joining_date DATE NOT NULL,
	salary DOUBLE NOT NULL,
	ssn VARCHAR(30) NOT NULL UNIQUE,
	PRIMARY KEY (id)
);
  
2. On project folder run : mvn package
3. Deploy war to Tomcat
4. Open : http://localhost:8080/SpringHibernateWeb/


The code is taken from : http://websystique.com/springmvc/spring-4-mvc-and-hibernate4-integration-example-using-annotations/