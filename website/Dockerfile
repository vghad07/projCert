FROM devopsedu/webapp 
LABEL maintainer="vikas@example.com"

RUN apt-get -qq update

VOLUME [ "/var/www/html" ]
WORKDIR /var/www/html
COPY ./website/ /var/www/html/

EXPOSE 80

ENTRYPOINT [ "/usr/sbin/apachectl" ]
CMD ["-D", "FOREGROUND"]
