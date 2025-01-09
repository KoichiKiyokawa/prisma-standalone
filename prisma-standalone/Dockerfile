FROM node:23.6.0 AS build
WORKDIR /work
RUN npm i -g pkg && npm i -D prisma@4.0.0 && pkg node_modules/prisma

FROM debian:stable-slim
COPY --from=build /work/prisma-linux /prisma
CMD ["/prisma"]