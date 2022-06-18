FROM node:16-alpine

ARG CACHE_BUST

RUN apk update && apk upgrade

WORKDIR /srv

# Copy stuff - refine this later on
COPY ./dist /srv/dist
COPY ./.env /srv/.env
COPY ./ormconfig.json /srv/ormconfig.json
COPY ./nest-cli.json /srv/nest-cli.json
COPY ./package.json /srv/package.json
COPY ./package-lock.json /srv/package-lock.json
COPY ./node_modules /srv/node_modules
