FROM ubuntu

MAINTAINER ambaticloud@gmail.com

WORKDIR /usr/apps/hello-docker/

RUN apt-get -y update

RUN apt-get install -y nodejs

RUN apt-get install -y npm

#RUN ln -s /usr/bin/nodejs /usr/bin/node

RUN npm install -g http-server

ADD . /usr/apps/hello-docker/

ADD index.html /usr/apps/hello-docker/index.html

HEALTHCHECK --interval=5m --timeout=3s CMD curl -f http://localhost:8282/ || exit 1

CMD ["http-server", "-s"]
