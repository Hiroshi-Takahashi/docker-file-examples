FROM centos:7

#wget install
RUN yum -y install wget

#java8 install
RUN wget --no-check-certificate --no-cookies --header "Cookie: oraclelicense=accept-securebackup-cookie" http://download.oracle.com/otn-pub/java/jdk/8u101-b13/jdk-8u101-linux-x64.tar.gz
RUN tar xvf jdk-8u101-linux-x64.tar.gz
RUN mkdir /opt/app/
RUN mv jdk1.8.0_101 /opt/app/

#activemq install
RUN wget https://archive.apache.org/dist/activemq/5.13.0/apache-activemq-5.13.0-bin.tar.gz
RUN tar xvzf apache-activemq-5.13.0-bin.tar.gz
RUN mv apache-activemq-5.13.0 /opt/app/

ENV PATH=$PATH:/opt/app/jdk1.8.0_101/bin
RUN echo $PATH


