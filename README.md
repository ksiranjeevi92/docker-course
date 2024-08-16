# Docker Course Resources

Solutions to the workbooks are inside the [**Complete** Docker Bootcamp](https://udemy-redirect-app.herokuapp.com/docker)

## lessons running codes

1. docker run --rm -v "/Users/workspace/docker-course/lesson-starter-projects/01-starter-code/:/app/" python:3.8.19-slim-bullseye python /app/python-app.py

2. docker run --rm -v "/Users/workspace/docker-course/lesson-starter-projects/ -02-starter-code/:/app/" --name java-app-container openjdk:11-jre-slim-buster java -cp /app/JavaApp.jar JavaApp

# Important command

- docker run -v "${pwd}:/app/" python:3.8.19-slim-bullseye python /app/python-app.py
- docker ps [comment] :running containers
- docker ps -a [comment]:all running containers
- docker rm [comment] <name> | <id>
- docker run -v "${pwd}:/app/" --nama python-app-container python:3.8.19-slim-bullseye python /app/python-app.py [comment]: nameing the container for easy access
- docker run --rm -v "${pwd}:/app/" --name python-app-container python:3.8.19-slim-bullseye python /app/python-app.py [comment]: nameing the container for easy access [comment] automatically removes container once it's finishes running.
- docker images [comment]:list all images from machine
- docker image rm [comment]<name>:<tag> | <image_id> to remove the image !ALERT for remove the comment should be `docker image rm <image_id>` not a images
- docker system prune -a [comment] : delete all cache
