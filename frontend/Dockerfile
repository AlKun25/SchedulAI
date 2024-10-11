# Use an official Node runtime as the base image
FROM node:22

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the frontend code
COPY . .

# Build the app for production
RUN npm run build

# Expose the port the app runs on
EXPOSE 8080

# Define the command to run the app
CMD ["npm", "run", "serve"]