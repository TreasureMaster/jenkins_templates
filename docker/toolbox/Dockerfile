FROM alpine

ENV PYTHONUNBUFFERED=1
# RUN apk add --no-cache curl wget busybox-extras netcat-openbsd python py-pip
RUN apk add --update --no-cache curl wget busybox-extras netcat-openbsd postgresql-client
# RUN apk add --no-cache python
RUN apk add --update --no-cache python3 && ln -sf python3 /usr/bin/python
RUN python3 -m ensurepip
# RUN apk add --no-cache py-pip
RUN pip3 install --no-cache --upgrade pip setuptools
RUN pip install awscli
# RUN apk --purge -v del py-pip
CMD tail -f /dev/null