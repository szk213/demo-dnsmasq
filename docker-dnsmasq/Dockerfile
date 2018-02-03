FROM alpine:3.7
RUN apk update && apk upgrade
RUN apk --no-cache add dnsmasq
ADD dnsmasq.conf /etc/dnsmasq.d/
ADD hosts /etc/dnsmasq.d/
EXPOSE 53 53/udp
ENTRYPOINT ["dnsmasq", "-k"]
