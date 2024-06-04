# ceseat-production-with-docker-compose
Meant to group all ceseat applications (&amp; DBs) and run them inside containers using docker compose

# How to run

```bash
# Create a network, which allows containers to communicate
# with each other, by using their container name as a hostname
docker network create [my_network]

# Build prod
docker compose --env-file ./.env.production.local -f docker-compose.prod.yml build

# Up prod in detached mode
docker compose --env-file ./.env.production.local -f docker-compose.prod.yml up -d
```
