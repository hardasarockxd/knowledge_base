# MYSQL Guide

### Enter
*mysql -u root -p*

### Show all databases
*SHOW databases;*

### Create database
*CREATE DATABASE name_of_database;*

### Delete database
*DROP DATABASE name_of_database;*

### Start to use database
*USE name_of_database;*

### Create table;
*CREATE TABLE name_of_table(
  id INT,
  name VARCHAR(30),
  surname VARCHAR(40),
  email VARCHAR(50)
  );*

### Delete table
*DROP TABLE name_of_table;*

### Show table
*DESC name_of_table;*

### Insert information to the table:
*INSERT INTO name_of_table VALUES (
  0, 'Yegor', 'Heiz', 'hardasarockgg@gmail.com'
  );*
*INSERT INTO name_of_table (name) VALUES (
  'Yegor2'
  );*

### Select information from table:
*SELECT * FROM name_of_table;* \n
*SELECT name, email FROM name_of_table WHERE name = 'Yegor'* \n
*SELECT name FROM name_of_table WHERE name = 'Yegor' OR age = 20;* \n
*SELECT name FROM name_of_table WHERE name = 'Yegor' AND age = 20;*
