# Dockerfile for Socket Service
FROM node:18

# Set the working directory inside the container
WORKDIR /usr/src/app

# Copy the package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Expose the port the socket service will run on (e.g., 5001 or any port you are using)
EXPOSE 5001

# Run the socket server
CMD ["node", "index.js"]
