FROM mariadb:latest

COPY docker-healthcheck.sh /usr/local/bin/docker-healthcheck
RUN chmod +x /usr/local/bin/docker-healthcheck

HEALTHCHECK CMD ["docker-healthcheck"]
