# docker-compose.yml
# https://patrickt.one/2020/01/14/building-a-database-sandbox.html
# Start a Postgres server with "docker-compose up -d". Stop the server with "docker-compose down".
# This file contains the settings outlined in the Postgres and Docker post [https://www.poeticoding.com/step-by-step-tutorial-to-build-a-phoenix-app-that-supports-user-uploads/#postgres-docker].
#  image: this selects the version of Postgres to run,
#  container_name: the name of the container,
#  ports: the port mapping between the local machine and container,
#  volumes: mounts the volume to the container to persist the data between runs,
#  environment: sets the Postgres password as an environment variable

version: "3"
services:
  db:
    image: postgres:11-alpine
    container_name: "postgres"
    ports:
      - "5432:5432"
    volumes:
      - postgres-dev:/var/lib/postgresql/data
    environment:
      - POSTGRES_PASSWORD=postgres
volumes:
  postgres-dev:
