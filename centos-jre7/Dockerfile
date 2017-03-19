FROM centos:latest

# Maintainer
MAINTAINER Chen Chiu

# Update system
RUN yum update -y
RUN yum install -y wget
RUN yum install -y unzip
RUN yum install -y tar

## Download and install Oracle JAVA JRE 1.7
RUN cd /tmp && wget -q --no-check-certificate -O /tmp/jre-8.tar.gz --no-cookies --no-check-certificate --header "Cookie: gpw_e24=http%3A%2F%2Fwww.oracle.com%2F; oraclelicense=accept-securebackup-cookie" http://download.oracle.com/otn-pub/java/jdk/8u121-b13/e9e7ea248e2c4826b92b3f075a80e441/jre-8u121-linux-x64.tar.gz
RUN tar -zxf /tmp/jre-8.tar.gz -C /opt
RUN rm /tmp/jre-8.tar.gz
RUN ln -s /opt/jre1.8.0_121 /opt/java

# Set up Java environment variables
ENV JAVA_HOME /opt/java
ENV PATH ${PATH}:${JAVA_HOME}/bin
