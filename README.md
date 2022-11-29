# vprofile-project

# Project to automate provisioning multiple vms locally with Vagrant. 




<h2>Description</h2>
The local MultiVM stack setup  will be created using nginx, tomcat, mariadb, memcache, rabbitmq


<br />


<h2>Languages and Utilities Used</h2>

- <b>Bash</b> 
- <b>Oracle VM Virtualbox 7.0 </b>
- <b>Vagrant boxes</b>
- <b>https://app.vagrantup.com/boxes/search</b>

<h2>Environments Used </h2>

- <b>Win 11</b>
- <b>Ubuntu 18 server</b>
- <b>centos7</b>

<h2>Program walk-through:</h2>


- edited the Vagrant.conf file to add the configuration setup steps for all servers <br/>
<br/>


<img width="651" alt="vagrant file setup" src="https://user-images.githubusercontent.com/85902399/204619140-89e2b3e7-70e9-4eeb-a087-4dd04f7e531f.png">




<br />
<br />

- once completed, verify the servers are running; 

<br/>


<img width="479" alt="vagrant up" src="https://user-images.githubusercontent.com/85902399/204619178-64a12f49-5a5a-4924-87d6-1e8d1b99501f.png">


<br />
<br />

- validation that the nodes can talk and hosts file are setup correctly;

<img width="499" alt="ssh web01 validation" src="https://user-images.githubusercontent.com/85902399/204619322-2805069c-d53d-4bf1-9d39-d69b9a4886d9.png">



<br />

# Building the backend 

<h3>db01 server - Mariadb setup</h3>

- setting up Mariadb and firewall settings on db01 server ;



<img width="734" alt="db setup" src="https://user-images.githubusercontent.com/85902399/204624525-ea7ff7f7-1598-44df-aa2f-f436c1b32559.png">



</p>

<h3>mc01 server - Memcache server</h3>

<br />
<br />

- setting up memcache and firewall settings on mc01 server ;


<img width="766" alt="memcached" src="https://user-images.githubusercontent.com/85902399/204629821-a638014a-fab9-4ad9-a7a2-413ff135429b.png">
<br />
<br />

- validating ip ports;


<br />

<img width="660" alt="mc validate port 11211" src="https://user-images.githubusercontent.com/85902399/204629911-2e3a1544-45a6-451e-a1fa-4de39ef45048.png">


<br />

<h3>mq01 server - Rabbitmq server</h3>

<br />
<br />


- setting up rabbitmq and firewall settings on mq01 server ;

<img width="871" alt="rabbitmq server" src="https://user-images.githubusercontent.com/85902399/204636527-f029e33c-8722-4afe-9bfc-1d3292294fb4.png">


<br />
<br />

<img width="730" alt="rabbitfw" src="https://user-images.githubusercontent.com/85902399/204637289-15b77655-720b-461f-b6ca-ed96e7ae6eb7.png">


<br />


# Building tomcat server

<br />
<br />
- setting up tomcat and firewall settings on app01 server ;

<img width="868" alt="tomcat" src="https://user-images.githubusercontent.com/85902399/204645377-aab1f6cd-6a06-42c1-b6df-292713bb3a68.png">

<br />
<br />

# Code build and deploy

<br />
<br />
- deploying app to app01 server;

<br />
<br />
<img width="876" alt="build code" src="https://user-images.githubusercontent.com/85902399/204649049-32050e2d-47b1-4339-8fb4-aaa5992f478a.png">


# Building Nginx server

<br />
<br />
- setting up nginx on web01 server ;

<img width="779" alt="nginx" src="https://user-images.githubusercontent.com/85902399/204651540-46dd70f2-7e95-4a9f-b468-7df0f85af902.png">


<br />
<br />


# Validating deployment

<br />
<br />
- Nginx webserver login using localhost ip;
<br />

<img width="952" alt="nginx website validate" src="https://user-images.githubusercontent.com/85902399/204654789-894461fd-cf1b-46ce-9580-1d75fb193384.png">


<br />
<br />


- db01 is working, since we can login;
<br />


<img width="953" alt="app validate login" src="https://user-images.githubusercontent.com/85902399/204654813-7ffc69ab-a5fe-44ce-8f77-9c92a5781ac3.png">


<br />
<br />

- validating rabbitmq(mq01) is working;
<br />

<img width="701" alt="rabbit01" src="https://user-images.githubusercontent.com/85902399/204654830-e3027214-3cd1-492b-b3fe-1dc76950cf51.png">

<br />
<br />

<img width="393" alt="rabbit02" src="https://user-images.githubusercontent.com/85902399/204654891-f5f52f36-8ad1-4e63-afa9-f3bffd95875f.png">



<br />
<br />
