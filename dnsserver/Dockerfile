FROM debian:13

RUN apt update  && apt install -y \
    procps \
    iproute2 \
    iputils-ping \
    bind9 \
    bind9utils \
    dnsutils \
    && rm -rf /var/lib/apt/lists/*

RUN mkdir -p /dns 

COPY entrypoint.sh /dns
RUN chmod a+x /dns/entrypoint.sh
EXPOSE 53
WORKDIR /var/cache/bind

CMD ["-g","-4"]

ENTRYPOINT ["/dns/entrypoint.sh"]