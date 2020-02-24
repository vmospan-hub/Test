FROM centos

RUN yum install -y httpd # web-assets-httpd

LABEL maintainer='vitalii.mospan'

ADD index.html /var/www/html/index.html
EXPOSE 80
ENTRYPOINT ["httpd"]
CMD ["-DFOREGROUND"]