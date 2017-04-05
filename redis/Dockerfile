FROM centos:centos6
MAINTAINER Redis

RUN yum -y update; yum clean all
RUN yum -y install epel-release; yum clean all
RUN yum -y install redis; yum clean all

EXPOSE 8081

CMD [ "redis-server" ]
