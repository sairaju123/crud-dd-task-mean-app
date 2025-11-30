# Use a lightweight Node image
FROM node:18-alpine
#create app directory
WORKDIR /app
# Install backend dependencies
COPY pacage*.json ./
# install
RUN npm install
# Copy the rest of the backend code
COPY . . 
# Expose backend port
EXPOSE 8080
# Start the Node.js server
CMD ["node", "server.js"]
