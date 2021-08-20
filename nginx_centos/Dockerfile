FROM centos:7
RUN yum install -y openssl
RUN yum install -y wget
RUN wget http://nginx.org/packages/centos/7/x86_64/RPMS/nginx-1.16.1-1.el7.ngx.x86_64.rpm
RUN rpm -i nginx-1.16.1-1.el7.ngx.x86_64.rpm
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
