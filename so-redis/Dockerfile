FROM redis:6-alpine
LABEL maintainer "Security Onion Solutions, LLC"
LABEL description="REDIS running in Docker container for use with Security Onion"
RUN addgroup -g 939 socore && adduser -D --uid 939 --ingroup socore socore

RUN chown 939:939 /data
VOLUME /data
WORKDIR /data
EXPOSE 6379
CMD ["redis-server"]
