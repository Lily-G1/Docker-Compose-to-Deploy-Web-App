# Docker-Compose-to-Deploy-Web-App
Define &amp; run a simple, multi-container web application using docker-compose

## To run:  
>> Install [Docker](https://docs.docker.com/engine/install/ubuntu/#set-up-the-repository)    
> $ git clone https://github.com/Lily-G1/Docker-Compose-to-Deploy-Web-App.git web-app  
> $ cd web-app  
> $ docker compose build  
> $ docker compose up -d  
>>  check browser with IP address or localhost:80. To test the app, fill form & submit  
>> To confirm that our app is connected to the backend, view the database to check for successful data entries:  
   > $ docker ps  
   > $ docker exec -it 'mysql container ID' /bin/bash  
    > # mysql -u root -p   (enter mysql password)  
       > mysql> use db;  
       > mysql> select * from test;		   --> to view table & confirm that form data has been entered successfully  
       > exit;		   --> to exit mysql  
    > # exit		   --> to exit container  
> $ docker compose down       --> stops & removes containers, images, volumes, etc created by docker compose up -d  
