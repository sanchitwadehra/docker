# Base image as node 14
FROM node:14

# Install nodemon globally
RUN npm install -g nodemon

# Set working directory inside container
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy application files to container
COPY . .

# Expose the application port (3000 in this case)
EXPOSE 3000

# Run the app with nodemon
CMD ["nodemon", "app.js"]
