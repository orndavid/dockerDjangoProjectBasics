# Docker Django Project Basics
A project that allows you to build an empty docker container with the read files mounted as  "volumes" so you can manipulate the website interactively.

The source of the project comes directly from  Very Academy (a youtube creator) and this specific setup comes from their video on the topic
- https://www.youtube.com/watch?v=e63EBEFJkH0
## Run 
Assuming you have docker installed (with docker-compose) [and docker active] you should be able to build a project using the following command 
```bash
docker-compose run --rm app django-admin startproject core . 
```
This will create the required files (an empty django project). 

The docker-compose.yml currently maps the ports as follows
- 8000:8000
So you should have an active service on 
- localhost:8000/

Good luck

## Requirements
This has only been tested on Linux, especially since docker is linux based and most servers run on linux anyway. The packages required to run this
- Docker
- Python
- docker-compose (tested using python package: pip install docker-compose)

