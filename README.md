- `docker compose up -d` run Docker compose to pull docker images and run docker container
- `docker images` verify docker images pulled
*`docker ps -a` verify docker container execution
*`doker logs mysql` connect to container interactive bash shell
*bash-4.4# `mysql -u root -p`
*Enter password: `uimm`
*mysql> `CREATE DATABASE DB;` create a new database
*mysql> `SHOW DATABASES;` show all database existing on the docker
*mysql> `SHOW TABLES FROM data_base;` show all tables existing on the data_base
*mysql> `USE db-test;` select the database to use
*mysql> `SELECT * FROM table_test;` request to display 
*mysql> `quit` exit mysql command line
*bash-4.4# `exit` qui bash shell prompt of container 
