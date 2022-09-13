FROM node:16-alpine as dev
WORKDIR /app
ENV NODE_ENV=development
COPY package.json yarn.lock ./
RUN yarn
COPY . .
