# MYSQL Guide

## Hints

### Enter
*mysql -u root -p*

### Show all databases
* *SHOW databases;*

### Create database
* *CREATE DATABASE name_of_database;*

### Delete database
* *DROP DATABASE name_of_database;*

### Start to use database
* *USE name_of_database;*

### Create table;
* *CREATE TABLE name_of_table(
  id INT AUTO_INCREMENT,
  name VARCHAR(30),
  surname VARCHAR(40),
  email VARCHAR(50),
  PRIMARY KET (id)
  );*

### Delete table
* *DROP TABLE name_of_table;*

### Show table
* *DESC name_of_table;*

### Insert information to the table:
* *INSERT INTO name_of_table VALUES (
  0, 'Yegor', 'Heiz', 'hardasarockgg@gmail.com'
  );*
* *INSERT INTO name_of_table (name) VALUES (
  'Yegor2'
  );*

### Select information from table:
* *SELECT * FROM name_of_table;*
* *SELECT name, email FROM name_of_table WHERE name = 'Yegor'*
* *SELECT name FROM name_of_table WHERE name = 'Yegor' OR age = 20;*
* *SELECT name FROM name_of_table WHERE name = 'Yegor' AND age = 20;*
* *SELECT * FROM name_of_table WHERE email '%com'*
* *SELECT * FROM name_of_table WHERE email '%gmail%'*
* *SELECT * FROM name_of_table WHERE email 'hard%'*
* *SELECT * FROM name_of_table WHERE email '_ard%'*

### Delete sth from table
* *DELETE FROM users WHERE name = 'Vlad'*

### Update sth in table
* *UPDATE name_of_table SET name = 'John' WHERE id = 2*

### Update table
* *ALTER TABLE users ADD COLUMN isSuperman BOOLEAN*

## Нормализация
* Столбец не может состоять из нескольких однотипных элементов
* Таблица не может состоять из нескольких однотипных полей  

## Связи
* Один к одному - когда одна запись из одной таблицы может быть связана только с одной записью из другой таблицы
* Один ко многим - когда одна запись из одной таблицы может быть связана с несколькими записями из другой таблицы  
* Многие ко многим - нужно создать доп таблицу, где будут связи один ко многим, ибо нет связи многие ко многим
