# pull official base image
FROM node:13.12.0-alpine

# set working directory
WORKDIR /app/client

# install app dependencies
COPY package*.json ./
RUN npm ci

# add app
COPY . .

# start app
CMD ["npm", "start"]