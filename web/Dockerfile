FROM tomcat:9.0-jre8

COPY ./tomcat-users.xml /usr/local/tomcat/conf/
COPY ./app/cool-memes.war /usr/local/tomcat/webapps/

CMD ["catalina.sh", "run"]
