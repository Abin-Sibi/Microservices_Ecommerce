# Use a specific Node.js version image, prefer a full Node.js image to avoid issues with alpine images
FROM node:22

# Set the working directory
WORKDIR /app/customer

# Copy package.json and package-lock.json first
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Expose the port your application will run on
EXPOSE 8001

# Start the application
CMD ["npm", "start"]
