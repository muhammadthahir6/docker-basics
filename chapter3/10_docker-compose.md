## Docker compose

+ a tool for defining and running multi-container Docker applications
+ use a YAML file to configure your application’s services


```
version: "3.9"  # optional since v1.27.0
services:       # docker services 
  web:          # service name , equivalent to --name web
    build: .    # docker build
    ports:      # posts
      - "5000:5000"
    volumes:    # volume info for the service 
      - .:/code
      - logvolume01:/var/log
  redis:
    image: redis
volumes:
  logvolume01: {}

```