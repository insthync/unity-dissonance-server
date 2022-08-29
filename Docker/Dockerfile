FROM ubuntu:18.04
LABEL maintainer="ittipon.bay@gmail.com"

COPY build/ /root/build/
COPY run.sh /run.sh

EXPOSE 3000

ENTRYPOINT ["/bin/bash", "/run.sh"]