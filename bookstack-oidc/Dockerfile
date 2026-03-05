FROM 10.1.1.4:3000/henryreed/bookstack:latest

RUN apk update && \
    apk add ca-certificates && \
    rm -rf /var/cache/apk/*

COPY root_ca.crt /usr/local/share/ca-certificates/root_ca.crt

RUN update-ca-certificates
