# Docker-Compose-to-Deploy-Web-App
Define &amp; run a simple, multi-container web application using docker-compose

## To run:  
> Install [Docker](https://docs.docker.com/engine/install/ubuntu/#set-up-the-repository)    
> $ git clone https://github.com/Lily-G1/Docker-Compose-to-Deploy-Web-App.git web-app  
> $ cd web-app  
> $ docker compose build  
> $ docker compose up -d  
> Check browser with IP address or localhost:80. To test the app, fill form & submit  

![Contact Form - Brave 6_13_2023 9_28_59 AM](https://github.com/Lily-G1/Docker-Compose-to-Deploy-Web-App/assets/104821662/826debca-09e3-4e6d-80af-0f87123528d0)  

> To confirm that our app is connected to the backend, view the database to check for successful data entries:  
   > $ docker ps  
   > $ docker exec -it 'mysql container ID' /bin/bash  
    > # mysql -u root -p   (enter mysql password)  
       > mysql> use db;  
       > mysql> select * from test;		   --> to view table & confirm that form data has been entered successfully  
       > exit;		   --> to exit mysql  
    > # exit		   --> to exit container  
  
![ubuntu@ip-172-31-92-33_ ~ 6_13_2023 9_31_17 AM](https://github.com/Lily-G1/Docker-Compose-to-Deploy-Web-App/assets/104821662/ad696c80-3d6c-4c3b-bac4-ef8b8c9bcc0a)  

> $ docker compose down       --> stops & removes containers, images, volumes, etc created by docker compose up -d  
