# Utilisez une image de base Node.js
FROM node:14

WORKDIR /app

COPY package*.json ./

RUN npm install

RUN npm install prom-client

ENV POSTER_DIR=../posters
COPY . .

EXPOSE 8080

CMD ["node", "server.js"]
