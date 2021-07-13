FROM centos:7 as rpm_centos7

RUN mkdir -p /extra && \
    yum install -y https://dev.mysql.com/get/mysql80-community-release-el7-3.noarch.rpm

RUN yum install --downloadonly mysql-community-server-8.0.23-1.el7 mysql-shell-8.0.23-1.el7 mysql-router-community-8.0.23-1.el7 --downloaddir=/extra/mysql-cluster

RUN yum install -y epel-release

RUN yum install --downloadonly redis-3.2.12-2.el7.x86_64 --downloaddir=/extra/redis

RUN yum install --downloadonly ruby-2.0.0.648-36.el7 rubygems-2.0.14.1-36.el7 --downloaddir=/extra/ruby

CMD [ "sleep", "360000000" ]    