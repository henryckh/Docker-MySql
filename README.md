# Docker-MySQL

Setup for a MySql docker using utf8 with phpmyadmin and initial data restore.

## Restore from database

The MySql docker image will run SQL files stored in the `/docker-entrypoint-initdb.d/`  
directory when you first launch a container.  
Restore the entire database by putting your database dump `schema.sql` into the directory.

## Config to support MySQL utf8

If you use `utf8` as the database content but haven't configured your database to use `utf8`,  
you maybe encouter encoding error.  
`my.cnf` contains the settings of utf8

## Config MySql

See the offical [MySql environment variables](https://hub.docker.com/_/mysql/) for more information.

## Result

Go to http://localhost:8080, with username: root, password: testing. A dump database is create from the `schema.sql` file.