FROM rhel7:7.5

MAINTAINER Rosthan Ngomssi ngomssi@gmail.com

LABEL DESCRIPTION="A basic Apache container on RHEL 7 UBI"

RUN yum install -y httpd && \
    yum clean all

RUN echo "hello from Dockerfile" > /usr/share/httpd/noindex/index.html

EXAPOSE 80

ENTRYPOINT ["httpd", "-D", "FOREGROUND"]


