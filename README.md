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
    ->  description TEXT NULL
    -> , Tcreated DATETIME NOT NULL,
    ->  creater VARCHAR(30) NULL,
    ->  profile VARCHAR(100) NULL,
    ->  PRIMARY KEY(id));
Query OK, 0 rows affected, 1 warning (0.13 sec)
`
