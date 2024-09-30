FROM node:11.4.0-alpine

RUN mkdir -p /usr/src/mockit-routes
WORKDIR /usr/src/mockit-routes

COPY package.json .
COPY package-lock.json .

RUN npm install

COPY . .

EXPOSE 3030

CMD ["npm", "start"]