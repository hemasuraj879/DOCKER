# Use nodejs official docker image
FROM node:latest

# Setting up workdir
WORKDIR /app

# Copy source code
COPY package.json .
COPY server.js .

# Install dependencies
RUN npm install

# Expose port number
EXPOSE 8080

# Command to start the application
CMD ["node", "server.js"]