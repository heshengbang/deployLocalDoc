FROM ubuntu:16.04
MAINTAINER heshengbang "yunshixin8521894@sohu.com"
ENV REFRESHED_AT 2018-04-05
ENV http_proxy 代理地址
ENV https_proxy 代理地址
 
RUN apt-get -qq update \
    && apt-get -qq install apache2 \
    && rm -rf /var/www/html/index.html \
    && mkdir -p $APACHE_RUN_DIR $APACHE_LOCK_DIR $APACHE_LOG_DIR
 
ENV APACHE_RUN_USER www-data
ENV APACHE_RUN_GROUP www-data
ENV APACHE_LOG_DIR /var/log/apache2
ENV APACHE_PID_FILE /var/run/apache2.pid
ENV APACHE_RUN_DIR /var/run/apache2
ENV APACHE_LOCK_DIR /var/lock/apache2

COPY . /var/www/html/
 
EXPOSE 80

ENTRYPOINT [ "/usr/sbin/apache2" ]
CMD ["-D", "FOREGROUND"]
