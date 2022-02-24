### Dockerized Prisma API (PostgreSQL)

dockerized Prisma REST API with PostgreSQL

Use this docker-compose as a simple way to have a containerized postgres instance (so you don't need to configure anything):

Installation
Requirements: docker

Store the following URL in an ENV variable

DATABASE_URL="postgresql://user:password@localhost:8432/development_db?schema=public"
Copy the datasource db config from the prisma/schema.prisma file to your prisma schema, so it uses the DATABASE_URL variable as the prisma db source, or just hardcode it

Run > docker-compose up in your terminal to start the service.