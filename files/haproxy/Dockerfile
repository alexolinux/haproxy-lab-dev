FROM haproxy:2.6

LABEL env="dev"
LABEL MANTAINER="alexmbarbosa"

USER root

RUN apt-get update -y && \
    apt-get install libcap2-bin -y && \
    rm -rf /var/lib/apt/lists/* && \
    setcap 'cap_net_bind_service=+ep' /usr/local/sbin/haproxy

USER haproxy

ENV DNS_TCP_ADDR=127.0.0.11
ENV DNS_TCP_PORT=53

COPY ./confs/haproxy.cfg /usr/local/etc/haproxy/haproxy.cfg
