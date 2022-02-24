# mysql relational database

## DATABASE which values in column is same

Example. (Duplication : creater and profile)

---



| id | topic      | description       | Tcreated            | creater | profile       |
|----|------------|-------------------|---------------------|---------|---------------|
|  1 | MYSQL      | MYSQL is ...      | 2022-02-24 09:08:19 | HHJ     | Hacker        |
|  2 | MongoDB    | MongoDB is ...    | 2022-02-24 09:18:54 | Jack    | Programmer    |
|  3 | SQL server | SQL server is ... | 2022-02-24 09:19:36 | Jack    | Programmer    |
|  4 | Python     | Python is ...     | 2022-02-24 09:20:45 | James   | Data analyzer |
|  5 | C          | C is ...          | 2022-02-24 09:21:13 | HHJ     | Hacker        |
|  6 | Go         | Go is ...         | 2022-02-24 09:28:57 | HHJ     | Hacker        |


---


## In relational database, it can join each tables

---

- **New topic table**


| id | title      | description       | Tcreated            | author_id |
|----|------------|-------------------|---------------------|-----------|
|  1 | MYSQL      | MYSQL is ...      | 2022-02-24 23:01:14 |         1 |
|  2 | MongoDB    | MongoDB is ...    | 2022-02-24 23:01:34 |         2 |
|  3 | SQL server | SQL server is ... | 2022-02-24 23:01:57 |         2 |
|  4 | Python     | Python is ...     | 2022-02-24 23:02:52 |         3 |
|  5 | C          | C is ...          | 2022-02-24 23:03:27 |         1 |
|  6 | Go         | Go is ...         | 2022-02-24 23:03:38 |         1 |


---

- **Author table**


| id | name  | profile       |
|----|-------|---------------|
|  1 | HHJ   | Hacker        |
|  2 | Jack  | Programmer    |
|  3 | James | Data analyzer |


---

_RENAME : RENAME [(table, database ...)] [before_name] TO [after_name]_

---

