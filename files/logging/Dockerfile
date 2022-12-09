
FROM alpine:3.17.0

RUN apk add --no-cache bash syslog-ng
RUN mkdir /sidecar

COPY conf/* /etc/syslog-ng/
COPY entrypoint.sh /entrypoint.sh

VOLUME ["/sidecar"]

CMD ["syslog-ng", "-F"]
ENTRYPOINT ["/entrypoint.sh"]