FROM node:17-alpine

WORKDIR /usr/src/app

COPY package*.json ./
RUN npm install
COPY index.html .
COPY server.js .

ENV PRODUCTS_SERVICE="products"
ENV SHOPPING_CART_SERVICE="shopping-cart"

EXPOSE 3000
CMD ["npm", "start"]
