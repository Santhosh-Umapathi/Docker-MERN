# Production

#------------------------------------
# Build Phase
#------------------------------------
## Base Image
FROM node:16-alpine as builder

## Specify the base working directory
WORKDIR '/app'

## Run Commands - Install Dependencies
COPY ./package.json ./
RUN npm install
COPY . .
RUN npm run build

#------------------------------------
# Run Phase
#------------------------------------
## Base Image
FROM nginx
EXPOSE 3000
COPY ./nginx/default.conf /etc/nginx/conf.d/default.conf
## Copy the build folder from above phase
COPY --from=builder /app/build /usr/share/nginx/html