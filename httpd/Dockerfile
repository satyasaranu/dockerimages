FROM centos:latest
RUN yum -y --setopt=tsflags=nodocs update && \
    yum -y --setopt=tsflags=nodocs install httpd && \
        yum clean all
EXPOSE 80
COPY index.html /var/www/html/
CMD ["/usr/sbin/apachectl","-DFOREGROUND"]

