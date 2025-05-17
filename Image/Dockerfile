FROM ubuntu:latest
RUN apt-get update && \
    apt-get install -y git bash curl jq && \
    rm -rf /var/lib/apt/lists/*
WORKDIR /opt
RUN git clone https://github.com/rsantomauro/CloudFare_DynDns.git . && \
    chmod +x cf_updateDNS
CMD ["./cf_updateDNS"]