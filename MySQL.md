# My SQL

## Relational DataBase

## Installtion on Ubuntu
```
sudo apt-get update -y
sudo apt-get upgrade -y

sudo apt install mysql-server -y

sudo mysql_secure_installation
```
- choose password type and 
- set password
- connect

```
sudo mysql -u root
```

## Viewing Database

```
show databases;
```

## creating Database

```
create database database_name;
```
## work with MySQl WorkBench
- Install MySQL Workbench from browser
- Easy to Monitor our databases
  - Administation Tab
  - Schemas tab
- You can check status of database from Schemas tab
- you can check server connection from adminstration tab

## Database Components
- Tables
- Views
- Stored Procedures
- Functions

## SQL Basic Commands
- To view all data from a table

```
select * from database.tablename;
```
- example

```
select * from world.city;
```
- modifications

### select command
- To view everything
- Note: Database must be selected

```
select * from table_name;

exanple

select * from city;
```
- To view particular column

```
select column_name1, column_name2
from table_name;

example

select Name, Country
from city;
```
- To add any arthmatic expression to column

```
select 
    column_name1,
    column_name2,
    column_name2 * 2
from table_name;

example

select 
    Name,
    Population,
    Population * 2
from city;
```
- To modify edited column name

```
select 
    column_name1,
    column_name2,
    column_name2 * 2 AS column_name
from table_name;

example

select 
    Name,
    Population,
    Population * 2 AS Strength
from city;
```

