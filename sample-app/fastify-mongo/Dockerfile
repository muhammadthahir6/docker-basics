FROM node:16-alpine
WORKDIR /usr/src/app
COPY package*.json ./
RUN npm install
COPY . .
# Run the web service on container startup.
CMD [ "npm", "start" ]