# Use the official Node.js image as the base image
FROM node:latest

# Create a directory to hold the application code inside the container
WORKDIR /app

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the website files to the container
COPY . .

# Expose the port on which the Node.js server will listen
EXPOSE 3000

# Start the Node.js server
CMD ["node", "server.js"]
