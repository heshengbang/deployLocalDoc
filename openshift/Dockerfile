FROM nginx:1.13.0
MAINTAINER heshengbang "yunshixin8521894@sohu.com"

RUN rm -rf /usr/share/nginx/html/index.html

COPY . /usr/share/nginx/html/
# COPY nginx.conf /etc/nginx/

EXPOSE 80 

ENTRYPOINT ["/usr/sbin/nginx","-g", "daemon off;"]
