# Use stable Node version (important for your old deps)
FROM node:16-alpine

# Set working directory
WORKDIR /app

# Copy package files
COPY package*.json ./

# Install dependencies
RUN npm install --legacy-peer-deps

# Copy app files
COPY . .

# Expose your backend port
EXPOSE 8000

# Start the app
CMD ["node", "app.js"]