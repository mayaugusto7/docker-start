# EXPOSE & HEALTHECHECK example
FROM ubuntu
ENV TZ="America"
RUN apt-get update
RUN apt-get install -y tzdata
RUN apt-get install -y apache2
RUN apt-get install -y curl
HEALTHCHECK CMD curl -f http://localhost/ || exit 1
EXPOSE 80
ENTRYPOINT ["apache2ctl", "-D", "FOREGROUND"]
