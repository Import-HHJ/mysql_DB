# mysql Structure

- DATABASE server (group of schema) -> DATABASE(schema) (group of table) -> Table(표)

> DATABASE server (group of schema)
> > DATABASE(schema) (group of table)
> > > Table(표)

# mysql database server connect

- `$ ./mysql -uroot -p` and Enter password

# mysql use schema

- create db : `CREATE DATABASE [DB_NAME];`

- delete db : `DROP DATABASE [DB_NAME];`

- show db : `SHOW DATABASES;`

- use db(before we use) : `USE [DB_NAME];`

# Table structure

> 행(column) `how much left to right`
> 열(row) `(how much top to down)`
> > Table

# mysql create table 

---

tip : use cheatsheet which is code somebody already made

---

 - MYSQL create topic table

 `mysql> CREATE TABLE topic(
    ->  id INT(11) NOT NULL AUTO_INCREMENT,
    ->  topic VARCHAR(100) NOT NULL,
    ->  description TEXT NULL,
    ->  Tcreated DATETIME NOT NULL,
    ->  creater VARCHAR(30) NULL,
    ->  profile VARCHAR(100) NULL,
    ->  PRIMARY KEY(id));
Query OK, 0 rows affected, 1 warning (0.13 sec)
`

---

varchar(size) : char which limited as size(until 255)
NOT NULL : need value
NULL : dont't have to need value
PRIMARY KEY : key value in id
DATETIME : (years:months:days hours:minutes:seconds)
TEXT : just can insert a lot of value

---

# mysql INSERT 

---

how to use INSERT data in table


1. INSERT INTO TABLE(field1, field2, field3, ...)

   VALUES (value1, value2, value3, ...)



2. INSERT INTO TABLE

   VALUES (value1, value2, value3, ...)


In case 2, it inserts values to table automatically

---

Example

`INSERT INTO topic(topic, description, Tcreated, creater, profile) VALUES("mysql", "mysql is ...", NOW(), "HHJ", "Hacker");`


DESC TABLE : describe and depict the table

# mysql SELECT

---

how to use SELECT syntax

`SELECT [columns] FROM [table] WHERE [condition] ORDER BY [sort_condition] LIMIT [show until numb you write]`


---

Example

`SELECT id, topic, Tcreated, creater FROM topic WHERE creater = "HHJ" ORDER BY id DESC LIMIT 2;`

ORDER BY [something] DESC :  mean sorted table great to low



