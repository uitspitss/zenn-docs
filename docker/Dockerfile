FROM node:14-alpine

ENV NODE_PATH /opt/node_modules

WORKDIR /workspace

# RUN apt-get -y update && apt-get install -y --no-install-recommends \
#         git \
#     && apt-get -y clean 
RUN apk update && apk add git


RUN npm init --yes \
    && npm install -g zenn-cli@latest \
    && npx zenn init
