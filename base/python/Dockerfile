FROM ghcr.io/svuctf/base/xinetd:alpine AS builder

FROM python:alpine

COPY --from=builder /usr/sbin/xinetd /usr/sbin/xinetd

RUN mkdir -p /etc/xinetd.d/ && \
    adduser -D -h /home/ctf ctf

CMD ["sleep", "infinity"]