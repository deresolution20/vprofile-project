# vprofile-project

<h2> see local-setup branch for manual setup</h2>

run Vagrant file in git bash using vagrant up.  This will create all the vms and run the individual shell scripts to provision them automatically.

This project will use Tomcat as an application server to host Java Web Application "Vprofile".
Nginx is used as a front-end server and used here as a load balancer.
MySQL is a SQL database server used for the backend for logins, etc.
RabbitMQ is an open source message broker.
MemCache is used here as a key value store for data (strings, objects) to store the results of database calls to help speed things up.

<br> </br>
<img width="951" alt="vprofilevagrantfile" src="https://user-images.githubusercontent.com/85902399/204665045-09df1b2c-f29d-43e4-933b-8fe41ad20feb.png">
