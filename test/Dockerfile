#FROM alpine:3.7

#RUN mkdir /app
#COPY /app/ ./app/

#ENTRYPOINT ["/app/1.sh"]

FROM alpine:3.7

RUN mkdir /app
RUN apk add dumb-init
COPY /app/ ./app/

ENTRYPOINT ["/usr/bin/dumb-init","--","/app/1.sh"]
