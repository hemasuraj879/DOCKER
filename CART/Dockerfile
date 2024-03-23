# Use an official Node.js image as base
FROM node:14.21.3-alpine3.17

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package*.json .

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY server.js .

# Expose the port on which the application will run
EXPOSE 8080

# Command to run the application
CMD ["node", "server.js"]
