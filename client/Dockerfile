# Use an official Node.js runtime as the base image
FROM node:alpine

# Create app directory
RUN mkdir -p /client

# Set the working directory in the container
WORKDIR /client

# Install app dependencies
COPY package.json /client/

# Install dependencies
RUN npm install

# Bundle app source
COPY . /client

# Expose the port the app runs on
EXPOSE 3000

# Command to run the application
CMD [ "npm", "start" ]
