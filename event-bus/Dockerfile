# Use an official Node runtime as a parent image
FROM node

# Set the working directory to /app
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the current directory contents into the container at /app
COPY . .

# Build the app 
EXPOSE 4005

# Set the command to start the app
CMD ["npm", "start"]
