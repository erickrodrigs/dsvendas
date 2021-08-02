FROM node:15.8.0-alpine

ENV PORT=3000

WORKDIR /usr/src/app

COPY package.json yarn.lock ./

RUN yarn install

COPY . .

USER node

EXPOSE ${PORT}

CMD yarn start
