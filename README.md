# docker-nginx-tomcat-server
Using docker-compose to deploy Nginx and Tomcat server in Docker . 

## how to use 

* pull nginx:1.13 and tomcat:8 by simply run 

		./build-image.sh

### config web 

update your /etc/hosts , and add 

		127.0.0.1 testa.com

		127.0.0.1 testb.com

		127.0.0.1 testc.com

### Nginx demo 

* run 

		docker-compose up -d

* open your browser , and visit http://testa.com and http://testb.com:5050,different page will be showed . 
		
* the output will be find in ./logs

### Tomcat demo

* run 

		docker-compose up -d 

	Open your browser , and visit http://localhost:8080					

* open your browser and visit http://localhost:8080/countuser-1.0-SNAPSHOT/ , you can find something produced by j2ee .		

	use commonds to enter tomcat terminal : 

		docker exec -it 容器ID/容器name /bin/bash	

### Nginx to Tomcat demo






