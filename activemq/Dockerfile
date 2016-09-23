FROM centos:7

#wget install
RUN yum -y install wget

#git install 
RUN yum -y install git

#java8 install
RUN wget --no-check-certificate --no-cookies --header "Cookie: oraclelicense=accept-securebackup-cookie" http://download.oracle.com/otn-pub/java/jdk/8u101-b13/jdk-8u101-linux-x64.tar.gz
RUN tar xvf jdk-8u101-linux-x64.tar.gz
RUN mkdir /opt/app/
RUN mv jdk1.8.0_101 /opt/app/
RUN rm -rf jdk-8u101-linux-x64.tar.gz 

#activemq install
RUN wget https://archive.apache.org/dist/activemq/5.13.0/apache-activemq-5.13.0-bin.tar.gz
RUN tar xvzf apache-activemq-5.13.0-bin.tar.gz
RUN mv apache-activemq-5.13.0 /opt/app/
RUN rm -rf apache-activemq-5.13.0-bin.tar.gz

#tomcat8 install 
RUN wget http://www-us.apache.org/dist/tomcat/tomcat-8/v8.5.5/bin/apache-tomcat-8.5.5.tar.gz
RUN tar xvzf apache-tomcat-8.5.5.tar.gz
RUN mv apache-tomcat-8.5.5 /opt/app/
RUN rm -rf apache-tomcat-8.5.5.tar.gz

ENV JAVA_HOME=/opt/app/jdk1.8.0_101
ENV PATH=$PATH:/$JAVA_HOME/bin
RUN echo $PATH


