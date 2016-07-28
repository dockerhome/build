# Dockerfile para wordpress com SSL

FROM wordpress

RUN echo "deb http://ftp.debian.org/debian jessie-backports main" > /etc/apt/sources.list.d/backports.list && \
	apt-get update && \
	apt-get install -y python-certbot-apache -t jessie-backports && \
	rm -rf /var/lib/apt/lists/* 

EXPOSE 80 443

#ENTRYPOINT["certbot"]
