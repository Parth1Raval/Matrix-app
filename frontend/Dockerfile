# Use a compatible Node version
FROM node:18-alpine

# Set working directory
WORKDIR /app

# Copy only package files first for caching
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the code
COPY . .

# Expose frontend port
EXPOSE 3000

# Start the app
CMD ["node", "app.js"]
