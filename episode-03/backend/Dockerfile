# Use the official Node.js image as base
FROM node:14-alpine

# Set working directory
WORKDIR /app

# Install Python and necessary build dependencies
RUN apk add --no-cache python3 make g++

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Expose port
EXPOSE 3000

# Start the application
CMD ["npm", "start"]
