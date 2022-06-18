FROM node:16-alpine

ARG CACHE_BUST

RUN apk update && apk upgrade

WORKDIR /srv

# Copy stuff - refine this later on
COPY ./.env /srv/.env
COPY ./package.json /srv/package.json
COPY ./package-lock.json /srv/package-lock.json
COPY ./node_modules /srv/node_modules
