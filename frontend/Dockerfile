# select a light weight node image 
FROM node:18-alpine
# Create working directory
WORKDIR /app
# Copy all the dependences 
COPY package*.json ./
# Install frontend dependencies
RUN npm install
# Copy the rest of angular project 
COPY . .
# Expose to port 
EXPOSE 8081
# Command
CMD ["npm", "run", "start", "--", "--host", "0.0.0.0", "--port", "8081"]
