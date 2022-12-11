FROM haproxy:2.6

LABEL env="dev"
LABEL MANTAINER="alexmbarbosa"

ENV DNS_TCP_ADDR=127.0.0.11
ENV DNS_TCP_PORT=53

COPY ./confs/haproxy.cfg /usr/local/etc/haproxy/haproxy.cfg
