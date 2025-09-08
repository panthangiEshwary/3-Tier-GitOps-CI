FROM node:22-alpine

WORKDIR /app

# Copy package files and install dependencies
COPY package*.json ./
RUN npm install --only=production

# Copy the rest of your app
COPY . .

# Expose the port your app runs on
EXPOSE 5000

# Command to start your backend
CMD ["node", "app.js"]

