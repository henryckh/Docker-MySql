FROM mysql:5.7
ADD my.cnf /etc/mysql/conf.d/mysqlutf8.cnf
CMD ["mysqld", "--character-set-server=utf8", "--collation-server=utf8_unicode_ci"]
ADD schema.sql /docker-entrypoint-initdb.d