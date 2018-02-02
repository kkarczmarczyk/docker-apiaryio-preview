# kkarczmarczyk/apiaryio-preview

This docker image is useful for apiary.io local development (live-preview) using docker-compose.

Example `docker-compose.yaml` file:

```yaml
version: '3'
services:
  web:
    image: kkarczmarczyk/apiaryio-preview
    volumes:
    - .:/tmp
    environment:
      APIB_PATH: example/test-api.apib
    ports:
     - "8080:8080"

```

