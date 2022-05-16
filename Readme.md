![image](https://wallpaperaccess.com/full/2982327.jpg)

# Docker MERN

Multi-Container MERN Application with Docker

## Features

- Docker Compose - Dev, Prod
- Docker File - Dev, Prod
- Build Images on Travis CI
- Push Images to Docker Hub
- CI/CD - Travis CI
- AWS - Beanstalk Hosting for Single Container
- AWS - Elastic Cache (Redis)
- AWS - RDS (Postgres)
- nginX Server for Production
- Deploy only from master branch
- Multiple - Stages, Containers
- Automatic changes from Local to Container (Volumes)

## Instructions

- Travis CI - Add the secrets into Travis Github Repo -> More Options -> Settings -> Environment Variables (Add key/value pairs)
- AWS - Create new Elastic Bean Stalk application, Create IAM user for Travis CI
- AWS - Copy all the required config fields
- AWS - Add security groups and update all services
