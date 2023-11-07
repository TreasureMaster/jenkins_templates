FROM alpine
# RUN apk add --no-cache curl wget busybox-extras netcat-openbsd python py-pip
RUN apk add --no-cache curl
RUN apk add --no-cache wget
RUN apk add --no-cache busybox-extras
RUN apk add --no-cache netcat-openbsd
RUN apk add --no-cache python
RUN apk add --no-cache py-pip
RUN pip install awscli
RUN apk --purge -v del py-pip
CMD tail -f /dev/null