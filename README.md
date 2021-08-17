# SQL & Relational Databases

Relational databases are the backbone of data science and the language that we use to communicate with them is called SQL. The SQL test is a common component for data-adjacenemnt jobs within industry, government and the education sector. It is a useful tool that some argue [spawned the field of data science](https://www.kdnuggets.com/gpspubs/sigkdd-explorations-kdd-10-years.html). Before Big Data was a thing, Knowledge Discovery in Databases (KDD) used simple SQL queries to investigate and understand the nature of the large amounts of data that were being collected by governments and companies. The humble SQL test now torments the budding data scientist as a right of passage in the job search process.

In this unit you will learn the basic ideas behind relational databases and SQL. You will setup a database in Amazon Web Services and then connect to it through RStudio. You will then load data into your database and run SQL queries on that data.

## Goals for this Unit

* Be able to discuss an overview of relational datanases and the purpose of SQL
* Be able to spin up an AWS instance and load a SQL database into it
* Be able to connect to the database through RStudio/R using the DBI package
* Be able to run basic SQL commands in RStudio using the RMySQL package

## Project: AWS Database and SQL

### Step by Step to setup AWS Account
* Log into your [AWS Management Console](https://console.aws.amazon.com)
* Locate `RDS` under the `Databases` heading
* Within Amazon RDS click `Create database`
* Under `Choose a database creation method` click `Standard Create`
* Under `Engine options` choose `MySQL`
* Under `Templates` choose `Free tier`
* Under `Settings` name your `DB instance identifier` as `database-1`
* Under `Credential settings` create a username and password combination and write it down (you will need it later)
* Under `Connectivity` expand `Additional connectivity configuration` to show additional menu items and make sure that `Publicly accessible` is checked `Yes`
* Expand the `Additional configuration` menu
* Under `Initial database name` write `oudb`
* Uncheck `Automatic backups`
* Click `Create database`
* Once the database is created, take a screenshot and add it to your repository

### Modify Security Group
* Under `Security Groups` click `Inbound` and then `Edit`
* Add the rule `SQL/Aurora` on `Port 3306` with the `Connection` of `MyIP`

### RStudio
* sql-project.Rmd - connected the Rmd to AWS MySQL Database and practiced SQL commands.

## Utilized the following resources

### Video 1
[![Introduction to Relational Databases & SQL](https://img.youtube.com/vi/G-rXRbdE7ow/0.jpg)](https://youtu.be/G-rXRbdE7ow)

[Transcript](https://github.com/la-process-and-theory/sql-db-setup/blob/master/hudk4051-sql-intro.rtf)

[Video Slide Deck](https://github.com/la-process-and-theory/sql-db-setup/blob/master/HUDK4051-SQL.pdf)

### Video 2
[![AWS Setup Instructions](https://img.youtube.com/vi/JnADtoprFMM/0.jpg)](https://youtu.be/JnADtoprFMM)

[SQL Cheat Sheet](https://mariadb.com/kb/en/basic-sql-statements/)

[Overview of Amazon Web Services](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/introduction.html)

[AWS](https://aws.amazon.com/)  

[AWS China](https://www.amazonaws.cn/?nc1=f_ls)
