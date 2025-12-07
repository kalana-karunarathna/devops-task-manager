FROM node:20-alpine

WORKDIR /app

# Copy package files
COPY package*.json ./

# Install dependencies (includes dev deps, good for tests)
RUN npm install

# Copy rest of the backend code
COPY . .

# Expose backend port
EXPOSE 3000

# Default command: start the server (for real usage)
CMD ["node", "src/server.js"]
