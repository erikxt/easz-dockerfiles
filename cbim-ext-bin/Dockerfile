FROM centos:7 as rpm_centos7

RUN mkdir -p /extra && \
    yum install -y https://dev.mysql.com/get/mysql80-community-release-el7-3.noarch.rpm

RUN yum install --downloadonly mysql-community-server-8.0.23-1.el7 mysql-shell-8.0.23-1.el7 mysql-router-community-8.0.23-1.el7 --downloaddir=/extra/mysql-cluster

CMD [ "sleep", "360000000" ]    