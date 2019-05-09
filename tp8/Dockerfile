FROM centos:7
RUN yum -y install epel-release
RUN yum -y update
RUN yum -y install nginx
ADD http://www.brainjar.com/java/host/test.html /usr/share/nginx/html/index.html
RUN chmod 644 /usr/share/nginx/html/index.html
#ADD ./index.html /opt
VOLUME /tmp/data
EXPOSE 80/tcp
CMD ["nginx", "-g", "daemon off;"]

