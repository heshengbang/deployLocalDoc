# mkdir /opt/apache
# cd /opt/apache
# vim Dockerfile
 
FROM golang:latest
MAINTAINER heshengbang "yunshixin8521894@sohu.com"

#ENV http_proxy 代理地址
#ENV https_proxy 代理地址
 
#RUN apt-get -qq update
#RUN apt-get -qq install apache2
 
#VOLUME [ "/var/www/html" ]
#WORKDIR /var/www/html
 
#ENV APACHE_RUN_USER www-data
#ENV APACHE_RUN_GROUP www-data
#ENV APACHE_LOG_DIR /var/log/apache2
#ENV APACHE_PID_FILE /var/run/apache2.pid
#ENV APACHE_RUN_DIR /var/run/apache2
#ENV APACHE_LOCK_DIR /var/lock/apache2
 
ENTRYPOINT ["sh", "-c", "godoc -http=:80"]
