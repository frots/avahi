FROM alpine:3.12
RUN apk add --update --no-cache avahi augeas

RUN mkdir /opt/avahi
COPY entrypoint.sh /opt/avahi/
RUN chmod +x /opt/avahi/entrypoint.sh

ENTRYPOINT ["/opt/avahi/entrypoint.sh"]

LABEL maintainer="matthew@thompsons.id.au"
