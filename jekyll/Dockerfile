# mkdir /opt/jekyll
# cd /opt/jekyll
# vim Dockerfile
 
FROM ubuntu:16.04
MAINTAINER heshengbang "trulyheshengbang@gmail.com"
ENV REFRESHED_AT 2018-04-05
 
RUN apt-get -qq update
RUN apt-get -qq install ruby ruby-dev build-essential nodejs
RUN gem install --no-rdoc --no-ri jekyll -v 2.5.3
RUN gem install rouge
 
VOLUME /data
VOLUME /var/www/html
WORKDIR /data
 
ENTRYPOINT [ "jekyll", "build", "--destination=/var/www/html" ]

