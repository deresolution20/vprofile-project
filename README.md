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

- setting up Mariadb on db01 server and firewall;



<img width="734" alt="db setup" src="https://user-images.githubusercontent.com/85902399/204624525-ea7ff7f7-1598-44df-aa2f-f436c1b32559.png">



 
</p>
