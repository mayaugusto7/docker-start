# ONBUILD example
FROM ubuntu
ENV TZ="America"
RUN apt-get update
RUN apt-get install -y tzdata
RUN apt-get install -y apache2
ONBUILD COPY *.html /var/www/html
EXPOSE 80
ENTRYPOINT ["apache2ctl", "-D", "FOREGROUND"]