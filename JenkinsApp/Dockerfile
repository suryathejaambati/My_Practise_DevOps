FROM jenkins/jenkins:lts
MAINTAINER SuryathejaAmbati
USER root
RUN apt-get -qqy update;apt-get install -qqy sudo
RUN echo "Jenkins ALL-NOPASSWD: ALL" >> /etc/sudoers
RUN wget http://get.docker.com/builds/Linux/x86_64/docker-latest.tgz
RUN tar -xvzf docker-latest.tgz
RUN mv docker/* /usr/bin
USER Jenkins
