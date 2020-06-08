## Container base
FROM node:11.2-alpine

## Container labels
LABEL version="1.0"

## Container environment variables
ENV NODE_ENV=${NODE_ENV:-development}

## Container setup
WORKDIR /app

ADD . .

## Container ports
EXPOSE 8080

## Container entry point default arguments (can be overwritten)
CMD [ "node", "index.js" ]