# syntax=docker/dockerfile:1

FROM node:16.13.1

ENV NODE_ENV=production
ENV HOST=db
ENV USER=postgres
ENV PASSWORD=psql7lOgin&
ENV DB=PernStackExample
ENV DIALECT=postgres
ENV PORT=80

WORKDIR /app

COPY ["./package.json", "./package-lock.json*", "./"]

RUN npm install --production

COPY . .

CMD [ "node", "server.js" ]

EXPOSE 80