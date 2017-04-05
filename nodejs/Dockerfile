FROM centos:centos6
MAINTAINER nodejs

RUN yum -y update; yum clean all
RUN yum -y install epel-release; yum clean all
RUN yum -y install nodejs npm; yum clean all
RUN yum -y install npm
ADD . /src

RUN cd /src; npm install

EXPOSE 8080

CMD [ "node", "/src/index.js" ]
