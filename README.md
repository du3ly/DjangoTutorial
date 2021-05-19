# DjangoTutorial (Poll application)

Following the tutorial from [Django](https://docs.djangoproject.com/en/3.2/intro/tutorial01/) on creating a poll app, but using Docker to host the environment.

Features:
- A public site that lets people view polls and vote in them.
- An admin site that lets you add, change, and delete polls.

Stack:
- Django
- PostgreSQL

## Requirements

- Docker

## Quick Start

Run docker-compose to start the app
```
docker compose up
```

Enter the URL (see below) in a browser to see the application running
localhost:8000/admin
localhost:8000/polls

## Docker commands

Access the PostgreSQL container
```
docker ps
psql -h localhost -p 5432 -d docker -U postgres --password
```

Executing commands through Docker
```
docker ps
docker exec -it <container_id_or_name> <command>

Ex:
docker exec -it 25b5806683d0 python manage.py shell
```
