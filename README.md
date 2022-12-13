# Learn MySQL

Basic Docker Compose file that will provide a mysql instance along with a web-based workbench tool in case you don't already have a db tool to connect to MySQL


## Docker Instructions:

How to start all services 

``` docker compose up -d ```

How to start just MySQL

``` docker compose up -d mysql ```


## Connect with MySQL Workbench via Browser:
Note: I've noticed on my M1 Mac this hasn't worked as well which is why I included Cloudbeaver below.
1. Start both services ``` docker compose up -d mysql mysql-workbench ```
2. In your browser go to ``` localhost:13000 ```
3. You'll need to add the MySQL instance connection.  
    - Host Name: mysql
    - user name: root
    - password: rootpassword
    - port: 13306

## Connect with Cloudbeaver
Notes: [Cloudbeaver](https://github.com/dbeaver/cloudbeaver)  is a web-based version of the very popular [dbeaver](https://github.com/dbeaver/dbeaver). 
        I preconfigured Cloudbeaver to connect to the MySQL database based on the docker compose committed, but you can see how the connection is configured.

1) Start up MySQL and Cloudbeaver in docker ``` docker compose up -d mysql cloudbeaver ```
2) Open browser to ``` localhost:18978 ```
3) Login info for Cloudbeaver
    -user name: cbadmin
    -password: cbadmin
4) Connection info (already configured, but if curious)
    - Host Name/Address: mysql
    - user name: root
    - password: rootpassword
    - port: 13306


## Connect with MySQL Workbench application

1. In terminal run the following command: ``` docker compose up -d mysql ```
2. Open MySQL Workbench
3. You'll need to add the MySQL instance connection.  
    - Host Name/Address: mysql
    - user name: root
    - password: rootpassword
    - port: 13306


## Notes:

Official MySQL tutorial -> https://dev.mysql.com/doc/mysql-tutorial-excerpt/8.0/en/

ANother great starting tutorial -> https://www.mysqltutorial.org
