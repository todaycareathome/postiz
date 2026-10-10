# Postiz in docker

The docker-compose.yml here is using Postgres in Host.

## Initialize
Since it use Postgres in Host, please create a Postgres database named `postiz_db` or any database name you like, and put it in the .env file.

It also has Redis in docker and Postiz is using 0. The Redis is available to Host and 1~15 are available in Host.


## Start
docker compose up
