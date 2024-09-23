# Use Node.js as the base image
FROM node:14

# Set the working directory
WORKDIR /app

# Install dependencies
COPY package*.json ./
RUN npm install

# Copy the rest of the source code
COPY . .

# Build the app
RUN npm run build

# Expose the frontend port
EXPOSE 3001

# Start the app
CMD ["npm", "start"]
