# Node.js base image
FROM node:21.6

# Set working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json to container
COPY ../package*.json ./

# Install dependencies
RUN npm install

# Copy all other application files to container
COPY . .

# Expose port 3034 (the port on which the Node.js application will run)
EXPOSE 3034

# Command to run the Node.js application
CMD ["npm", "start"]
