FROM alpine
RUN apk add curl wget busybox-extras 
RUN apk add curl wget netcat-openbsd 
RUN apk add curl wget python 
RUN apk add curl wget py-pip
RUN pip install awscli
RUN apk --purge -v del py-pip
CMD tail -f /dev/null
