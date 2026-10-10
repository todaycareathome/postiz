# Postiz in docker

The docker-compose.yml here is using Postgres in Host. Both Postiz and temporal using the very same Host Postgres.
Redis is available to Host.

## Initialize
Since it use Postgres in Host, please create a Postgres database named `postiz_db` or any database name you like, and put it in the .env file. There is a `.env.example` available to start, and you can put all social media credentials in it. I soft-link it to the parent directory to avoid push to Github.

Postiz is using Redis DB0. Other Redis DB (1~15) are available to Host.


## Start
```
docker compose up -d --remove-orphans
```

## Debug
Check Postiz log for error
```
docker compose logs postiz | grep -iE "error|fail|exception"
```
