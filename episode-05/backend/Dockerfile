# Use an official Node.js runtime as the base image
FROM node:14

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to the working directory
COPY backend/package*.json ./

# Install backend dependencies
RUN npm install

# Copy the backend source code to the container
COPY backend/ .

# Expose port 8000 to the outside world
EXPOSE 8000

# Command to run the backend application
CMD ["npm", "start"]
