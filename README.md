# Login-PhP-with-Sql

# Creating the Database and setting-up Tables
# For this part, you will need to access your MySQL database, either using phpMyAdmin or your preferred MySQL database management application.

# Follow the below instructions if you're using phpMyAdmin.

## Navigate to: http://localhost/phpmyadmin/
## Click the Databases tab at the top
## Under Create database, enter phplogin in the text box
## Select utf8_general_ci as the collation
## Click Create
## You can use your own database name, but for this tutorial, we'll use phplogin.

## What we need now is an accounts table as this will store all the accounts (usernames, passwords, emails, etc) that are registered with the system.

## Click the database on the left side panel (phplogin) and execute the following SQL statement:

## CREATE TABLE IF NOT EXISTS `accounts` (
## 	`id` int(11) NOT NULL AUTO_INCREMENT,
##  	`username` varchar(50) NOT NULL,
##   	`password` varchar(255) NOT NULL,
 ##  	`email` varchar(100) NOT NULL,
 ##    PRIMARY KEY (`id`)
## ) ENGINE=InnoDB AUTO_INCREMENT=2 DEFAULT CHARSET=utf8;

## INSERT INTO `accounts` (`id`, `username`, `password`, `email`) VALUES (1, 'test', '$2y$10$SfhYIDtn.iOuCW7zfoFLuuZHX6lja4lF4XA4JqNmpiH/.P3zB8JCa', 'test@test.com');


# THEN GO TO LOGIN PAGE:  
## Username: test 
## Password: test