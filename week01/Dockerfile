# Use an official Node.js runtime as the base image
FROM node:18

# Set the working directory in the container
WORKDIR /src

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install application dependencies
RUN npm install

# Copy the rest of the application code to the container
COPY . .

# Expose a port (if your application listens on a specific port)
EXPOSE 8080

# Define the command to run your application
CMD [ "npm", "start" ]
