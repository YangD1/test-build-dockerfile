FROM centos
MAINTAINER YoungDee
RUN yum update -y
RUN rpm -Uvh http://nginx.org/packages/centos/7/noarch/RPMS/nginx-release-centos-7-0.el7.ngx.noarch.rpm
RUN yum install -y nginx
RUN yum -y install gcc gcc-c++ autoconf pcre pcre-devel make automake
RUN yum -y install wget httpd-tools vim
RUN cd /opt;mkdir app download logs work backup
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
