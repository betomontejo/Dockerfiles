FROM ubuntu:trusty
RUN apt-get update
RUN apt-get install -y software-properties-common python-software-properties
RUN add-apt-repository ppa:webupd8team/java
RUN apt-get update
RUN apt-get install -y vim
RUN apt-get install -y wget
RUN apt-get install -y curl
RUN apt-get install -y unzip
RUN echo oracle-java8-installer shared/accepted-oracle-license-v1-1 select true | /usr/bin/debconf-set-selections
RUN apt-get install -y oracle-java8-installer
RUN wget http://downloads.typesafe.com/typesafe-activator/1.2.3/typesafe-activator-1.2.3-minimal.zip -P /opt
RUN cd /opt && unzip typesafe-activator-1.2.3-minimal.zip
RUN echo `/opt/activator-1.2.3-minimal/activator list-templates`
