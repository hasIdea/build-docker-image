FROM tomcat:8.5
VOLUME /tmp
ADD ROOT.war /usr/local/tomcat/webapps
EXPOSE 8099
ENTRYPOINT ["/usr/local/tomcat/bin/catalina.sh","run"]