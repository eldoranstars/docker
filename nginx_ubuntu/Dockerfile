FROM ubuntu:18.04
RUN apt-get update \
&& apt-get -y dist-upgrade
RUN apt-get -y install net-tools nginx
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
