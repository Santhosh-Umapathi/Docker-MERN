# Production

## Base Image
FROM node:alpine

## Specify the base working directory
WORKDIR '/app'

## Run Commands - Install Dependencies
COPY ./package.json ./
RUN npm install
COPY . .

## Start Command - Starting the Image
CMD ["npm", "run", "start"]
