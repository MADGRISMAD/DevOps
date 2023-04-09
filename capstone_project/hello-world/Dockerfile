# Use an official Node.js runtime as a parent image
FROM node:16.13.1

# Set the working directory in the container to /app
WORKDIR /app

# Copy the package.json and package-lock.json files to the container
COPY package*.json ./

# Install the app's dependencies using npm
RUN npm install

# Copy the rest of the app's code to the container
COPY . .

# Build the app for production
RUN npm run build

# Expose port 3000 for the app to listen on
EXPOSE 3000

# Set the startup command to run the app using npm
CMD ["npm", "start"]
