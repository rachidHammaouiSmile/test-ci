FROM node:9.2-alpine

RUN apk add --no-cache su-exec && \
    apk add --update bash && \
    apk add --update make && \
    apk add --update patch && \
    addgroup bar && \
    adduser -D -h /home -s /bin/sh -G bar foo

ADD entrypoint.sh /entrypoint.sh

RUN chmod +x /entrypoint.sh

ENTRYPOINT ["sh" , "/entrypoint.sh"]