FROM node:24.12.0-alpine

WORKDIR /app

COPY docker/vuejs/*.sh /usr/local/bin/

COPY vuejs-app/vueApp/ /app/

RUN find /app -maxdepth 2 -type f | sort

RUN chmod +x /usr/local/bin/*.sh

EXPOSE 5173