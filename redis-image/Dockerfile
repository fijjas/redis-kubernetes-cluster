FROM alpine:3.4

RUN apk add --no-cache redis sed bash

COPY master.conf /redis-master/redis.conf
COPY slave.conf /redis-slave/redis.conf
COPY run.sh /run.sh

RUN chmod +x /run.sh

CMD [ "/run.sh" ]
ENTRYPOINT [ "bash", "-c" ]
