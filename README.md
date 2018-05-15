# docker-nginx-tomcat-server
Using docker-compose to deploy Nginx and Tomcat server in Docker . 

## how to use 

* pull nginx:1.13 and tomcat:8 by simply run 

		./build-image.sh

### config web 

update your /etc/hosts , and add 

		127.0.0.1 testa.com

		127.0.0.1 testb.com

### Nginx demo 

* run 

		docker-compose up -d

* open your browser , and visit http://testa.com and http://testb.com:5050,different page will be showed . 
		
* the output will be find in ./logs

### Nginx to Tomcat demo

