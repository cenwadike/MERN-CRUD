# Use an official Node.js runtime as the base image
FROM node:alpine

# Create app directory
RUN mkdir -p /server

# Set the working directory in the container
WORKDIR /server

# Install app dependencies
COPY package.json /server/

# Install dependencies
RUN npm install

# Bundle app source
COPY . /server/

# Expose the port the app runs on
EXPOSE 8080

# Command to run the application
CMD [ "npm", "run" "start" ]
