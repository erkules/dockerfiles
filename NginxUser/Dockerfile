FROM ubuntu:18.04
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update
RUN apt-get install -y nginx-light
RUN useradd -G tty -u 2222 www 
COPY ./nginx.conf /etc/nginx/nginx.conf
COPY ./default    /etc/nginx/sites-enabled/default
RUN ln -sf /dev/stdout /var/log/nginx/access.log && ln -sf /dev/stderr /var/log/nginx/error.log
RUN chown www: -R /var/cache
RUN chown www:  /var/lib/nginx
USER 2222
ENTRYPOINT ["/usr/sbin/nginx","-g","daemon off;"]
