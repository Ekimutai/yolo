# Use an official Node.js runtime as a parent image
FROM node:16-alpine

# Set the working directory to /app
WORKDIR /app

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code to the container
COPY . .

# Expose port 5000
EXPOSE 5000

# Start the application
CMD [ "npm", "run", "start" ]

# docker build -t yolo-backend .
# docker run -it -p 5000:5000 yolo-backend