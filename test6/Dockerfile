FROM centos

RUN yum install -y httpd # web-assets-httpd

LABEL maintainer='vitalii.mospan'

RUN ln -s /dev/stdout /var/log/httpd/access_log
RUN ln -s /dev/stderr /var/log/httpd/error_log

ADD index.html /var/www/html/index.html
EXPOSE 80
ENTRYPOINT ["httpd"]
CMD ["-DFOREGROUND"]