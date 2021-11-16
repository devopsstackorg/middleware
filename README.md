$git clone https://github.com/devopsstackorg/middleware.git

$cd middleware

$docker image build -t <image_name> .

$docker container run -d -it --name <container_name> -p 8080:8080 <image_name>

Optional steps: $docker exec -it <container_name> bash

vi /usr/local/tomcat/webapps/conf/server.xml

$git clone https://github.com/krishnamaram2/WebApp.git

$docker cp WebApp/binary/Student.war <container_name>:/usr/local/tomcat/webapps/

$sh /usr/local/tomcat/bin/catalina.sh start

Reference: https://www.cprime.com/resources/blog/deploying-your-first-web-app-to-tomcat-on-docker/
