## Create a docker image

Lets create a docker image for the app fastify-mongo

+ create a Dockerfile in the fasitfy-mongo directory

```bash

cd sample-app/fastify-mongo

touch Dockerfile

## copy the contents

```

Dockerfile
```
FROM node:16-alpine
WORKDIR /usr/src/app
COPY package*.json ./
RUN npm install
COPY . .
# Run the web service on container startup.
CMD [ "npm", "start" ]
```


### Build docker image

```
docker build -t fastify-mongo:v1 -f Dockerfile .
```

### Run the image

```
docker run -e MONGO_BASE="172.17.0.2:27017"  fastify-mongo:v1
```
