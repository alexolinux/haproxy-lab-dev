FROM haproxy:2.6

LABEL env="dev"
LABEL MANTAINER="alexmbarbosa"

EXPOSE 80
EXPOSE 1936

COPY ./confs/haproxy.cfg /usr/local/etc/haproxy/haproxy.cfg
