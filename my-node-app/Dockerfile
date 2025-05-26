# Use official Node.js image
FROM node:16

# Create app directory inside container
WORKDIR /usr/src/app

# Copy package.json and install dependencies
COPY package*.json ./
RUN npm install

# Copy remaining app files
COPY . .

# Expose port 3000 to outside world
EXPOSE 3000

# Command to run the app
CMD ["node", "index.js"]