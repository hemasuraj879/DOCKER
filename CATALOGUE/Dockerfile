# Use a official nodejs image
FROM node

# Setting up workdir
WORKDIR /app

# Copy source code
COPY .js .
COPY .json .

# Install the dependencies
RUN npm Install

# Setting up environment variables
ENV MONGO=true

# Expose port number
EXPOSE 8080

# Command to run the application
CMD ["node", "server.js"]

