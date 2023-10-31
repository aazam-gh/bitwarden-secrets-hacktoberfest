FROM node:16

WORKDIR /test-app
COPY package.json .
RUN npm install
COPY . .
CMD npm start
