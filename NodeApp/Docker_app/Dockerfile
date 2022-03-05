FROM node:14-alpine

# Creating app directory
WORKDIR /usr/src/app

# Installing app dependencies
COPY package*.json .

RUN npm install
# building code for production
# RUN npm ci --only=production

# Bundle app source
COPY . .

EXPOSE 8081
CMD [ "node", "server.js" ]