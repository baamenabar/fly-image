FROM node:0.12

ENV REDIS_COMMANDER_VERSION=0.3.2

RUN npm config set registry http://registry.npmjs.org/ && \
  npm i -g --unsafe-perm --no-optional redis-commander@$REDIS_COMMANDER_VERSION

EXPOSE 8081

CMD ["redis-commander", "--redis-host", "redis-service"]