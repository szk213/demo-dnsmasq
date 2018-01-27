FROM alpine:3.7
RUN apk update -y && apk upgrade -y
RUN apk --no-cache add dnsmasq
EXPOSE 53 53/udp
ENTRYPOINT ["dnsmasq", "-k"]