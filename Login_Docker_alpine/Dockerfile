FROM alpine

MAINTAINER ambaticloud@gmail.com

WORKDIR /usr/apps/hello-docker/

RUN apk update

RUN apk add nodejs

RUN apk add npm

#RUN ln -s /usr/bin/nodejs /usr/bin/node

RUN npm install -g http-server

ADD . /usr/apps/hello-docker/

ADD index.html /usr/apps/hello-docker/index.html

CMD ["http-server", "-s"]
