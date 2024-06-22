# ceseat-production-with-docker-compose
Meant to group all ceseat applications (&amp; DBs) and run them inside containers using docker compose

# How to run

```bash

# Build prod
docker compose --env-file ./.env.production.local -f docker-compose.prod.yml build

# Up prod in detached mode
docker compose --env-file ./.env.production.local -f docker-compose.prod.yml up -d
```
