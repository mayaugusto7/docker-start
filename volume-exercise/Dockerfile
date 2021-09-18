# VOLUME example
FROM ubuntu
ENV TZ="America"
RUN apt-get update
RUN apt-get install -y tzdata
RUN apt-get install -y apache2
VOLUME ["/var/log/apache2"]