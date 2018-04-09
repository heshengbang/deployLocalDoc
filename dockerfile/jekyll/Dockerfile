# mkdir /opt/jekyll
# cd /opt/jekyll
# vim Dockerfile
 
FROM ubuntu:16.04
MAINTAINER heshengbang "yunshixin8521894@sohu.com"
ENV REFRESHED_AT 2018-04-05
ENV http_proxy 代理地址
ENV https_proxy 代理地址
 
RUN apt-get -qq update
RUN apt-get -qq install ruby ruby-dev build-essential nodejs
RUN gem sources --add https://gems.ruby-china.org/ --remove https://rubygems.org/
RUN gem sources -l
RUN gem install --no-rdoc --no-ri jekyll -v 3.7.3
RUN gem install rouge
RUN gem install jekyll-redirect-from
 
VOLUME /data
VOLUME /var/www/html
WORKDIR /data
 
ENTRYPOINT [ "jekyll", "build", "--destination=/var/www/html" ]

