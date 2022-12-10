FROM haproxy:2.6

LABEL env="dev"
LABEL MANTAINER="alexmbarbosa"

# https://github.com/docker-library/haproxy/issues/170#issuecomment-968219682
USER root
RUN setcap 'cap_net_bind_service=+ep' /usr/local/sbin/haproxy

USER haproxy

EXPOSE 80

COPY ./confs/haproxy.cfg /usr/local/etc/haproxy/haproxy.cfg