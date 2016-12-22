FROM htakahashi77786/centos7
MAINTAINER Hirohshi Takahashi
RUN yum -y install wget
RUN yum -y install unzip
RUN yum -y install java-1.7.0-openjdk
RUN mkdir /opt/app/
WORKDIR /opt/app
RUN wget http://www-us.apache.org/dist/servicemix/servicemix-7/7.0.0.M3/apache-servicemix-7.0.0.M3.zip
RUN unzip apache-servicemix-7.0.0.M3.zip

