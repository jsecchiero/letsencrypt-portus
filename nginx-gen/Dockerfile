FROM jwilder/docker-gen:latest

ADD https://raw.githubusercontent.com/jwilder/nginx-proxy/master/nginx.tmpl /etc/docker-gen/templates/nginx.tmpl
RUN mkdir -p /etc/nginx/conf.d
RUN { \
      echo 'server_tokens off;'; \
      echo 'client_max_body_size 4g;'; \
    } > /etc/nginx/conf.d/custom.conf
