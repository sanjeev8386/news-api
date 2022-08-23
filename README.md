# Coreyo

1. clone the repo and checkout to `dev` branch
2. Assuming you have installed nodejs `v14.19.1` and `yarn`
3. do `yarn` in root directory for installing all required dependencies
4. create env file in root directory and update the latest env 

## Guide to install mysql because used mysql database
1. Run `sudo apt update` to update the package index
2. To mysql run `sudo apt install mysql-server` this will install mysql server in your system
3. Run `sudo systemctl start mysql.service` to start mysql service
4. Run `sudo mysql -u root -p` and enter your system password
5. Run `ALTER USER 'root'@'localhost' IDENTIFIED WITH caching_sha2_password BY 'you_mysql_password';` to update your mysql root user password
6. Run `flush privileges;` and then `quit;`
7. Restart mysql server using `sudo service mysql restart`

## After installing mysql or (if you have mysql already in your local)
1. Run `mysql -u root -p` and enter your mysql root user password
2. Run `create database your_database_name` this will create database in mysql 
3. Now run `yarn knex:migrate:latest` to create the required tables in the database

## Install redis in your local machine(if you don't have already follow below commands)
1. Run `sudo apt update`
2. Run `sudo apt install redis-server` to install redis
3. Run `sudo nano /etc/redis/redis.conf` 
4. edit `supervised no` to `supervised systemd`

## Now we are done with setup Let run the poject
```
yarn start
```

This will create build from the source code and serves the requests.

## Download postman collection from [Here](https://www.getpostman.com/collections/78aeec678e3f25e7388d)

## Download postman collection from [here](https://documenter.getpostman.com/view/17725459/VUqrNcYh)

### Happy Coding!!!
