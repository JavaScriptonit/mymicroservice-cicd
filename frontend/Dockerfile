FROM node:17-alpine

WORKDIR /usr/src/app

COPY package*.json ./
RUN npm install
COPY index.html .
COPY server.js .

ENV PRODUCTS_SERVICE="host.docker.internal"
ENV SHOPPING_CART_SERVICE="host.docker.internal"

EXPOSE 3000
CMD ["npm", "start"]
