FROM alpine
RUN apk add curl wget busybox-extras 
RUN apk add curl wget netcat-openbsd 
ENV PYTHONUNBUFFERED=1
RUN apk add --update --no-cache python3 && ln -sf python3 /usr/bin/python
RUN python3 -m ensurepip
RUN pip3 install --no-cache --upgrade pip setuptools
RUN apk add curl wget py-pip
RUN pip install awscli
RUN apk --purge -v del py-pip
CMD tail -f /dev/null
