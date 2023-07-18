# Tomcat_CMD
Tomcat_CMD
http://www.mithuntechnologies.com/devops/DevOpsToolsMithunTechnologies.html
https://www.youtube.com/watch?v=pSxWoCJRRco&t=1468s
=================================================================
sudo amazon-linux-extras enable corretto8
sudo yum install java-1.8.0-amazon-corretto
yum install java-1.8.0-openjdk -y
java -version
============================================================
cd /opt
wget https://dlcdn.apache.org/tomcat/tomcat-9/v9.0.78/bin/apache-tomcat-9.0.78.zip
unzip apache-tomcat-9.0.78.zip
yum install unzip -y
cd apache-tomcat-9.0.78
ls -l
cd bin/
chmod u+x *.sh
pwd
/opt/apache-tomcat-9.0.78/bin
ln -s /opt/apache-tomcat-9.0.78/bin/startup.sh /usr/bin/startTomcat
ln -s /opt/apache-tomcat-9.0.78/bin/shutdown.sh /usr/bin/stopTomcat
cd /opt
startTomcat
cd webapps
cd manager
ls
cd META-INF
ls
context.xml
vi context.xml
stopTomcat
startTomcat
========================================================================
<!--  <Valve className="org.apache.catalina.valves.RemoteAddrValve"
  allow="127\.\d+\.\d+\.\d+|::1|0:0:0:0:0:0:0:1" /> -->
========================================================================
stopTomcat
startTomcat
cd /opt/apache-tomcat-9.0.78
ls
cd conf
vi tomcat-users.xml
<user username="tomcat" password="password" roles="admin-gui,manager-gui"/>
username= tomcat
password= password

