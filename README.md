# Learn MySQL

Basic Docker Compose file that will provide a mysql instance along with a web-based workbench tool in case you don't already have a db tool to connect to MySQL


# Docker Instructions:

How to start both services 

docker compose up -d

How to start just MySQL

docker compose up -d mysql


# Connect with MySQL Workbench via Browser:

1. In your browser go to localhost:13000
2. You'll need to add the MySQL instance connection.  
    a. Use your computer IP address (i.e. 10.x.x.x or 192.168.x.x)
    b. user name: root
    c. password: rootpassword
    d. port: 13306

# Connect with MySQL Workbench application

1. Open MySQL Workbench
2. You'll need to add the MySQL instance connection.  
    a. Use your computer IP address (i.e. 10.x.x.x or 192.168.x.x)
    b. user name: root
    c. password: rootpassword
    d. port: 13306