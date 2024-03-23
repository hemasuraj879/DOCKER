# Use nodejs official docker image
FROM node:latest

# Setting up workdir
WORKDIR /app

# Copy source code
COPY package.json .
COPY server.js .

# Install dependencies
RUN npm install

# Command to start the application
CMD ["node", "server.js"]