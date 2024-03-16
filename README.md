# WebServerAlpineOS
Web Server Lightweight  on Alpine OS  for ARM64 

From Docker-Hub [webserveralpine](https://hub.docker.com/r/masihgurutkj/webserveralpine)
  
    PHP Version 8.3.3 
    MariaDB Version 10.5 
    NGINX/1.25.4) 
    PHPMyAdmin

Standar Running [Docker-Hub]
  
    docker pull masihgurutkj/webserveralpine:arm64.1.0
    
A. DIRECTORY
----------------------

webserveralpine
   
    - docker-compose.yml
    - index.php
    - nginx.conf
    - web/

B. STEP [ BUILD - RUN DOCKER-COMPOSE ]
-------------------------------
1. Download
   
    git clone https://github.com/otnamrehus/webserveralpin.git
  
    cd webserveralpine

2. Build docker-compose
   
        docker build -t webserveralpine . 
        #or use it
        docker build --platform linux/arm64 -t webserveralpine .   #opsional use "-platform linux/arm64"

3. Run [Stack] docker-compose
   
        docker-compose -p 'webserveralpine' up --build

4. Stop [Stack] docker-compose
   
        docker-compose -p 'webserveralpine' stop     # or use CTRL+C on Console

5. Clear [Stack] docker-compose
   
        docker-compose -p 'webserveralpine' down

C. RUN BROWSER
-------------------------------

1. Web
   
        http://IP_ADDRESS:7080
 
2. PHPMyAdmin
   
        http://IP_ADDRESS:7081
 
