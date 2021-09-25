# WORKDIR, COPY and ADD example
FROM ubuntu:latest
ARG UBUNTU_FRONTEND="noninteractive"
ENV TZ="America"
RUN apt-get update
RUN apt-get install -y tzdata
RUN apt-get install -y apache2
WORKDIR /var/www/html
COPY index.html .
ADD https://www.docker.com/sites/default/files/d8/2019-07/Moby-logo.png ./logo.png
CMD ["ls"]